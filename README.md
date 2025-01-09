
-- Carl Hub Brookhaven Script

local CarlHub = Instance.new("ScreenGui")
local MainFrame = Instance.new("Frame")
local MenuFrame = Instance.new("ScrollingFrame")

-- Configure Main GUI
CarlHub.Name = "CarlHub"
CarlHub.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

MainFrame.Name = "MainFrame"
MainFrame.Parent = CarlHub
MainFrame.BackgroundColor3 = Color3.fromRGB(30, 30, 45)
MainFrame.Position = UDim2.new(0.5, -250, 0.5, -175)
MainFrame.Size = UDim2.new(0, 500, 0, 350)

local TitleLabel = Instance.new("TextLabel")
TitleLabel.Parent = MainFrame
TitleLabel.BackgroundColor3 = Color3.fromRGB(40, 40, 60)
TitleLabel.Size = UDim2.new(1, 0, 0, 40)
TitleLabel.Font = Enum.Font.GothamBold
TitleLabel.Text = "Carl Hub - Brookhaven"
TitleLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TitleLabel.TextSize = 24

MenuFrame.Name = "MenuFrame"
MenuFrame.Parent = MainFrame
MenuFrame.BackgroundColor3 = Color3.fromRGB(35, 35, 50)
MenuFrame.Position = UDim2.new(0, 10, 0, 50)
MenuFrame.Size = UDim2.new(1, -20, 1, -60)
MenuFrame.CanvasSize = UDim2.new(0, 0, 2, 0)

local function createButton(name, callback, yPos)
    local button = Instance.new("TextButton")
    button.Size = UDim2.new(0, 200, 0, 40)
    button.Position = UDim2.new(0.5, -100, 0, yPos)
    button.BackgroundColor3 = Color3.fromRGB(60, 60, 90)
    button.Text = name
    button.TextColor3 = Color3.fromRGB(255, 255, 255)
    button.Font = Enum.Font.GothamSemibold
    button.TextSize = 16
    button.Parent = MenuFrame
    
    button.MouseButton1Click:Connect(callback)
    
    local UICorner = Instance.new("UICorner")
    UICorner.CornerRadius = UDim.new(0.1, 0)
    UICorner.Parent = button
end

-- Create feature buttons
createButton("Infinite Money", function()
    print("Attempting to modify money...")
end, 10)

createButton("Unlock All Houses", function()
    print("Attempting to unlock houses...")
end, 60)

createButton("Speed Boost", function()
    local player = game.Players.LocalPlayer
    if player.Character then
        player.Character.Humanoid.WalkSpeed = 32
    end
end, 110)

createButton("High Jump", function()
    local player = game.Players.LocalPlayer
    if player.Character then
        player.Character.Humanoid.JumpPower = 100
    end
end, 160)

local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 30, 0, 30)
CloseButton.Position = UDim2.new(1, -35, 0, 5)
CloseButton.BackgroundColor3 = Color3.fromRGB(255, 50, 50)
CloseButton.Text = "X"
CloseButton.TextColor3 = Color3.fromRGB(255, 255, 255)
CloseButton.Parent = MainFrame

CloseButton.MouseButton1Click:Connect(function()
    CarlHub:Destroy()
end)

local UICorner = Instance.new("UICorner")
UICorner.CornerRadius = UDim.new(0.02, 0)
UICorner.Parent = MainFrame
-- Carl Hub Brookhaven Script

local CarlHub = Instance.new("ScreenGui")
local MainFrame = Instance.new("Frame")
local MenuFrame = Instance.new("ScrollingFrame")

-- Configure Main GUI
CarlHub.Name = "CarlHub"
CarlHub.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

MainFrame.Name = "MainFrame"
MainFrame.Parent = CarlHub
MainFrame.BackgroundColor3 = Color3.fromRGB(30, 30, 45)
MainFrame.Position = UDim2.new(0.5, -250, 0.5, -175)
MainFrame.Size = UDim2.new(0, 500, 0, 350)

local TitleLabel = Instance.new("TextLabel")
TitleLabel.Parent = MainFrame
TitleLabel.BackgroundColor3 = Color3.fromRGB(40, 40, 60)
TitleLabel.Size = UDim2.new(1, 0, 0, 40)
TitleLabel.Font = Enum.Font.GothamBold
TitleLabel.Text = "Carl Hub - Brookhaven"
TitleLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TitleLabel.TextSize = 24

MenuFrame.Name = "MenuFrame"
MenuFrame.Parent = MainFrame
MenuFrame.BackgroundColor3 = Color3.fromRGB(35, 35, 50)
MenuFrame.Position = UDim2.new(0, 10, 0, 50)
MenuFrame.Size = UDim2.new(1, -20, 1, -60)
MenuFrame.CanvasSize = UDim2.new(0, 0, 2, 0)

local function createButton(name, callback, yPos)
    local button = Instance.new("TextButton")
    button.Size = UDim2.new(0, 200, 0, 40)
    button.Position = UDim2.new(0.5, -100, 0, yPos)
    button.BackgroundColor3 = Color3.fromRGB(60, 60, 90)
    button.Text = name
    button.TextColor3 = Color3.fromRGB(255, 255, 255)
    button.Font = Enum.Font.GothamSemibold
    button.TextSize = 16
    button.Parent = MenuFrame
    
    button.MouseButton1Click:Connect(callback)
    
    local UICorner = Instance.new("UICorner")
    UICorner.CornerRadius = UDim.new(0.1, 0)
    UICorner.Parent = button
end

-- Create feature buttons
createButton("Infinite Money", function()
    print("Attempting to modify money...")
end, 10)

createButton("Unlock All Houses", function()
    print("Attempting to unlock houses...")
end, 60)

createButton("Speed Boost", function()
    local player = game.Players.LocalPlayer
    if player.Character then
        player.Character.Humanoid.WalkSpeed = 32
    end
end, 110)

createButton("High Jump", function()
    local player = game.Players.LocalPlayer
    if player.Character then
        player.Character.Humanoid.JumpPower = 100
    end
end, 160)

local CloseButton = Instance.new("TextButton")
CloseButton.Size = UDim2.new(0, 30, 0, 30)
CloseButton.Position = UDim2.new(1, -35, 0, 5)
CloseButton.BackgroundColor3 = Color3.fromRGB(255, 50, 50)
CloseButton.Text = "X"
CloseButton.TextColor3 = Color3.fromRGB(255, 255, 255)
CloseButton.Parent = MainFrame

CloseButton.MouseButton1Click:Connect(function()
    CarlHub:Destroy()
end)

local UICorner = Instance.new("UICorner")
UICorner.CornerRadius = UDim.new(0.02, 0)
UICorner.Parent = MainFrame# Carl-hub

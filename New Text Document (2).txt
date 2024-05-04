-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local Menu1 = Instance.new("Frame")
local UIGradient = Instance.new("UIGradient")
local TextLabel = Instance.new("TextLabel")
local INY = Instance.new("TextButton")
local exit = Instance.new("TextButton")
local openmenu = Instance.new("Frame")
local openmenubutton = Instance.new("ImageButton")

--Properties:

ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Menu1.Name = "Menu1"
Menu1.Parent = ScreenGui
Menu1.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Menu1.BorderColor3 = Color3.fromRGB(0, 0, 0)
Menu1.BorderSizePixel = 0
Menu1.Position = UDim2.new(0.222696245, 0, 0.302729517, 0)
Menu1.Size = UDim2.new(0, 290, 0, 239)
Menu1.Active = true
Menu1.Visible = true
Menu1.Draggable = true

UIGradient.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(76, 76, 76)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(53, 53, 53))}
UIGradient.Rotation = 90
UIGradient.Parent = Menu1

TextLabel.Parent = Menu1
TextLabel.BackgroundColor3 = Color3.fromRGB(29, 29, 29)
TextLabel.BorderColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BorderSizePixel = 0
TextLabel.Size = UDim2.new(0, 290, 0, 50)
TextLabel.Font = Enum.Font.SourceSansBold
TextLabel.Text = "Flying Demon Piece - - BY.HOANGLONG"
TextLabel.TextColor3 = Color3.fromRGB(194, 129, 0)
TextLabel.TextSize = 19.000
TextLabel.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.TextWrapped = true

INY.Name = "INY"
INY.Parent = Menu1
INY.BackgroundColor3 = Color3.fromRGB(85, 170, 255)
INY.BorderColor3 = Color3.fromRGB(0, 0, 0)
INY.BorderSizePixel = 0
INY.Position = UDim2.new(0.334482759, 0, 0.426778257, 0)
INY.Size = UDim2.new(0, 95, 0, 55)
INY.Font = Enum.Font.SourceSansBold
INY.Text = "ON"
INY.TextColor3 = Color3.fromRGB(0, 0, 0)
INY.TextSize = 30.000
INY.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
INY.TextStrokeTransparency = 0.000
INY.MouseButton1Down:Connect(function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()
end)

exit.Name = "exit"
exit.Parent = Menu1
exit.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
exit.BorderColor3 = Color3.fromRGB(0, 0, 0)
exit.BorderSizePixel = 0
exit.Position = UDim2.new(0.872413695, 0, 0.88702929, 0)
exit.Size = UDim2.new(0, 37, 0, 27)
exit.Font = Enum.Font.SourceSansBold
exit.Text = "x"
exit.TextColor3 = Color3.fromRGB(0, 0, 0)
exit.TextSize = 30.000
exit.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
exit.TextStrokeTransparency = 0.000
exit.MouseButton1Down.Connect(function()
	Menu1.Visible = false
	openmenu.Visible = true
end)

openmenu.Name = "openmenu"
openmenu.Parent = ScreenGui
openmenu.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
openmenu.BorderColor3 = Color3.fromRGB(0, 0, 0)
openmenu.BorderSizePixel = 0
openmenu.Position = UDim2.new(0, 0, 0.303970218, 0)
openmenu.Size = UDim2.new(0, 160, 0, 106)
openmenu.Active = true
openmenu.Draggable = true

openmenubutton.Name = "openmenubutton"
openmenubutton.Parent = openmenu
openmenubutton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
openmenubutton.BorderColor3 = Color3.fromRGB(0, 0, 0)
openmenubutton.BorderSizePixel = 0
openmenubutton.Position = UDim2.new(-0.00274124136, 0, -0.00348648941, 0)
openmenubutton.Size = UDim2.new(0, 160, 0, 106)
openmenubutton.Image = "http://www.roblox.com/asset/?id=17377278546"
openmenubutton.MouseButton1Down:Connect(function()
	Menu1.Visible = true
	openmenu.Visible = false
end)

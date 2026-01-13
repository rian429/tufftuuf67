-- Delta Executor Optimized: Pink Glass Custom Edition
-- Theme: Pink Glass | Editable Seconds
-- ADDED: DRAG TOGGLE + BLOXSTRAP INSTALL BUTTON
-- ADDED: UI WIDTH (100–700px) + UI HEIGHT (50–350px)
-- OTHER LOGIC UNCHANGED

local Player = game:GetService("Players").LocalPlayer
local PlayerGui = Player:WaitForChild("PlayerGui")
local UIS = game:GetService("UserInputService")

if PlayerGui:FindFirstChild("DeltaPinkCustom") then
	PlayerGui.DeltaPinkCustom:Destroy()
end

local ScreenGui = Instance.new("ScreenGui")
ScreenGui.Name = "DeltaPinkCustom"
ScreenGui.Parent = PlayerGui
ScreenGui.ResetOnSpawn = false
ScreenGui.IgnoreGuiInset = true

local FreezeDuration = 0.4
local DRAG_ENABLED = true

-- UI SIZE STATE
local UI_WIDTH = 200
local UI_HEIGHT = 75

------------------- UI ELEMENTS -------------------

local Main = Instance.new("TextButton")
Main.Size = UDim2.new(0, UI_WIDTH, 0, UI_HEIGHT)
Main.Position = UDim2.new(0.5, -UI_WIDTH/2, 0.4, 0)
Main.BackgroundColor3 = Color3.fromRGB(255, 20, 147)
Main.BackgroundTransparency = 0.5
Main.BorderSizePixel = 0
Main.Text = "FREEZE"
Main.Font = Enum.Font.GothamBold
Main.TextSize = 24
Main.TextColor3 = Color3.new(1,1,1)
Main.AutoButtonColor = false
Main.Parent = ScreenGui

local MainStroke = Instance.new("UIStroke")
MainStroke.Thickness = 3
MainStroke.Color = Color3.fromRGB(255,105,180)
MainStroke.Parent = Main

local DragToggle = Instance.new("TextButton")
DragToggle.Size = UDim2.new(0,40,0,18)
DragToggle.Position = UDim2.new(1,-45,0,5)
DragToggle.BackgroundColor3 = Color3.fromRGB(255,255,255)
DragToggle.BackgroundTransparency = 0.8
DragToggle.Text = "ON"
DragToggle.Font = Enum.Font.GothamBold
DragToggle.TextSize = 12
DragToggle.TextColor3 = Color3.fromRGB(255,20,147)
DragToggle.Parent = Main

DragToggle.MouseButton1Click:Connect(function()
	DRAG_ENABLED = not DRAG_ENABLED
	DragToggle.Text = DRAG_ENABLED and "ON" or "OFF"
end)

local SettingBtn = Instance.new("TextButton")
SettingBtn.Size = UDim2.new(0,25,0,25)
SettingBtn.Position = UDim2.new(0,5,0,5)
SettingBtn.BackgroundColor3 = Color3.fromRGB(255,255,255)
SettingBtn.BackgroundTransparency = 0.8
SettingBtn.Text = "⚙"
SettingBtn.TextSize = 15
SettingBtn.Parent = Main

local SideMenu = Instance.new("Frame")
SideMenu.Size = UDim2.new(0,160,0,210)
SideMenu.Position = UDim2.new(1,10,0,0)
SideMenu.BackgroundColor3 = Color3.fromRGB(30,0,15)
SideMenu.BackgroundTransparency = 0.3
SideMenu.Visible = false
SideMenu.Parent = Main

local SideStroke = Instance.new("UIStroke")
SideStroke.Color = Color3.fromRGB(255,105,180)
SideStroke.Thickness = 2
SideStroke.Parent = SideMenu

-- SECONDS
local InputTitle = Instance.new("TextLabel")
InputTitle.Text = "SET SECONDS"
InputTitle.Size = UDim2.new(1,0,0,18)
InputTitle.BackgroundTransparency = 1
InputTitle.TextColor3 = Color3.fromRGB(255,105,180)
InputTitle.Font = Enum.Font.GothamBold
InputTitle.TextSize = 10
InputTitle.Parent = SideMenu

local InputBox = Instance.new("TextBox")
InputBox.Size = UDim2.new(0.8,0,0,24)
InputBox.Position = UDim2.new(0.1,0,0.12,0)
InputBox.BackgroundColor3 = Color3.fromRGB(0,0,0)
InputBox.BackgroundTransparency = 0.5
InputBox.Text = tostring(FreezeDuration)
InputBox.TextColor3 = Color3.new(1,1,1)
InputBox.Font = Enum.Font.GothamBold
InputBox.TextSize = 12
InputBox.Parent = SideMenu

-- UI WIDTH
local WidthLabel = Instance.new("TextLabel")
WidthLabel.Text = "UI WIDTH (100–700)"
WidthLabel.Size = UDim2.new(1,0,0,18)
WidthLabel.Position = UDim2.new(0,0,0.32,0)
WidthLabel.BackgroundTransparency = 1
WidthLabel.TextColor3 = Color3.fromRGB(255,105,180)
WidthLabel.Font = Enum.Font.GothamBold
WidthLabel.TextSize = 10
WidthLabel.Parent = SideMenu

local WidthBox = Instance.new("TextBox")
WidthBox.Size = UDim2.new(0.8,0,0,24)
WidthBox.Position = UDim2.new(0.1,0,0.42,0)
WidthBox.BackgroundColor3 = Color3.fromRGB(0,0,0)
WidthBox.BackgroundTransparency = 0.5
WidthBox.Text = tostring(UI_WIDTH)
WidthBox.TextColor3 = Color3.new(1,1,1)
WidthBox.Font = Enum.Font.GothamBold
WidthBox.TextSize = 12
WidthBox.Parent = SideMenu

-- UI HEIGHT
local HeightLabel = Instance.new("TextLabel")
HeightLabel.Text = "UI HEIGHT (50–350)"
HeightLabel.Size = UDim2.new(1,0,0,18)
HeightLabel.Position = UDim2.new(0,0,0.56,0)
HeightLabel.BackgroundTransparency = 1
HeightLabel.TextColor3 = Color3.fromRGB(255,105,180)
HeightLabel.Font = Enum.Font.GothamBold
HeightLabel.TextSize = 10
HeightLabel.Parent = SideMenu

local HeightBox = Instance.new("TextBox")
HeightBox.Size = UDim2.new(0.8,0,0,24)
HeightBox.Position = UDim2.new(0.1,0,0.66,0)
HeightBox.BackgroundColor3 = Color3.fromRGB(0,0,0)
HeightBox.BackgroundTransparency = 0.5
HeightBox.Text = tostring(UI_HEIGHT)
HeightBox.TextColor3 = Color3.new(1,1,1)
HeightBox.Font = Enum.Font.GothamBold
HeightBox.TextSize = 12
HeightBox.Parent = SideMenu

-- INSTALL BLOXSTRAP
local InstallBtn = Instance.new("TextButton")
InstallBtn.Size = UDim2.new(0.9,0,0,28)
InstallBtn.Position = UDim2.new(0.05,0,0.82,0)
InstallBtn.BackgroundColor3 = Color3.fromRGB(255,105,180)
InstallBtn.BackgroundTransparency = 0.2
InstallBtn.Text = "INSTALL BLOXSTRAP"
InstallBtn.Font = Enum.Font.GothamBold
InstallBtn.TextSize = 12
InstallBtn.TextColor3 = Color3.new(1,1,1)
InstallBtn.Parent = SideMenu

------------------- LOGIC -------------------

InputBox.FocusLost:Connect(function()
	local v = tonumber(InputBox.Text)
	if v then FreezeDuration = v else InputBox.Text = tostring(FreezeDuration) end
end)

WidthBox.FocusLost:Connect(function()
	local v = tonumber(WidthBox.Text)
	if v then
		UI_WIDTH = math.clamp(v, 100, 700)
		Main.Size = UDim2.new(0, UI_WIDTH, 0, UI_HEIGHT)
		Main.Position = UDim2.new(0.5, -UI_WIDTH/2, Main.Position.Y.Scale, Main.Position.Y.Offset)
	else
		WidthBox.Text = tostring(UI_WIDTH)
	end
end)

HeightBox.FocusLost:Connect(function()
	local v = tonumber(HeightBox.Text)
	if v then
		UI_HEIGHT = math.clamp(v, 50, 350)
		Main.Size = UDim2.new(0, UI_WIDTH, 0, UI_HEIGHT)
	else
		HeightBox.Text = tostring(UI_HEIGHT)
	end
end)

SettingBtn.MouseButton1Click:Connect(function()
	SideMenu.Visible = not SideMenu.Visible
end)

InstallBtn.MouseButton1Click:Connect(function()
	loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-OP-bloxstrap-mobile-71317"))()
end)

local IsFreezing = false
local function TriggerFreeze()
	if IsFreezing then return end
	IsFreezing = true
	Main.Text = "FREEZING..."
	task.wait(0.01)
	local Start = os.clock()
	while os.clock() - Start < FreezeDuration do
		for i = 1, 5000000 do local _ = i * i end
	end
	Main.Text = "FREEZE"
	IsFreezing = false
end

local dragging, dragInput, dragStart, startPos
local function update(input)
	local delta = input.Position - dragStart
	Main.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
end

Main.InputBegan:Connect(function(input)
	if not DRAG_ENABLED then return end
	if (input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch)
		and UIS:GetFocusedTextBox() == nil then
		dragging = true
		dragStart = input.Position
		startPos = Main.Position
		input.Changed:Connect(function()
			if input.UserInputState == Enum.UserInputState.End then dragging = false end
		end)
	end
end)

Main.InputChanged:Connect(function(input)
	if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
		dragInput = input
	end
end)

UIS.InputChanged:Connect(function(input)
	if dragging and DRAG_ENABLED and input == dragInput then update(input) end
end)

Main.MouseButton1Click:Connect(TriggerFreeze)

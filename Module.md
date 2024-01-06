# SECRET LIBRARY
your dirty mind its just a gender😡

# Booting The Library
```lua
local sex = loadstring(game:HttpGet('https://raw.githubusercontent.com/CludeHub/CludeHub/main/CludeHub'))()
```


# Creating Window
```lua
local Window = sex:Create('title of the Library','title of game','TEST')

-- title of The Script
-- title of the game
-- title of the unknown
```


# Creating Tab
```lua
local ExampleTab = Window:CreateTab('Tab 1','earth')

-- make tab title of the tab
-- name of the earth
```


# Creating Button
```lua
ExampleTab:CreateButton("Button",function()	   
 print('press button')    
end)

-- name of the button
-- second function of the button
-- anything script on function not a toggle
```


# Creating CheckBox Toggle
```lua
ExampleTab:CreateToggle("Toggle",false,function(val)     
	print('toggle',val)     
end)

-- name of the toggle button
-- function of the toggle
-- name String Script not a button script
```


# Creating Slider
```lua
ExampleTab:CreateSlider("Slider",1,100,10,function(val)     
	print('slider',val)     
end)

-- Name of slider
-- function of the slider
-- speed of anything else
```


# Create Label
```lua
ExampleTab:CreateLabel("Label")
```


# Creating KeyBind
```lua
ExampleTab:CreateKeybind("Keybind",Enum.KeyCode.E,function(val)     
	print('keybind',val)      
end)

-- title of keybind
-- Enum the letter of the keyboard
-- function of the keybind
```


# Creating Window Button Earth
```lua
Window:CreateButton('earth',false,function(val)        
	print('set time')
	if val then
		Window:Notify('Time Change','Night',1.5)
		game:GetService('TweenService'):Create(game:GetService('Lighting'),TweenInfo.new(0.5),{ClockTime = 0}):Play()
	else
		Window:Notify('Time Change','Day',1.5)
		game:GetService('TweenService'):Create(game:GetService('Lighting'),TweenInfo.new(0.5),{ClockTime = 14}):Play()
	end    
end)
```


# Creating Window Button ADS
```lua
Window:CreateButton('ads',false,function(val)      
	print('fov change')
	if val then
		Window:Notify('FOV Change','120',1)
		game:GetService('TweenService'):Create(workspace.CurrentCamera,TweenInfo.new(0.5),{FieldOfView = 120}):Play()
	else
		Window:Notify('FOV Change','70',1)
		game:GetService('TweenService'):Create(workspace.CurrentCamera,TweenInfo.new(0.5),{FieldOfView = 70}):Play()
	end    
end)
```
# Make a Loader
```lua
-- By Paul Paras
-- loader
-- Instances:

local cka = Instance.new("ScreenGui")
local frame = Instance.new("Frame")
local titler = Instance.new("TextLabel")
local button = Instance.new("TextButton")

--Properties:

cka.Name = "cka"
cka.Parent = game.CoreGui

frame.Name = "frame"
frame.Parent = cka
frame.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
frame.Transparency = 0
frame.BorderColor3 = Color3.fromRGB(0, 0, 155)
frame.BorderSizePixel = 3
frame.Position = UDim2.new(0, 120.746, 0, 0)
frame.Size = UDim2.new(0, 481, 0, 272)

titler.Name = "titler"
titler.Parent = frame
titler.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
titler.BorderColor3 = Color3.fromRGB(255, 0, 0)
titler.BorderSizePixel = 0
titler.Size = UDim2.new(0, 481, 0, 40)
titler.Font = Enum.Font.SourceSans
titler.Text = "☄️Welcome To CludeHub Script☄️"
titler.TextColor3 = Color3.fromRGB(255, 255, 255)
titler.TextSize = 28.000

button.Name = "button"
button.Parent = frame
button.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
button.Transparency = 0.1
button.BorderColor3 = Color3.fromRGB(0, 128, 0)
button.BorderSizePixel = 0
button.Position = UDim2.new(0, 154, 0, 134)
button.Size = UDim2.new(0, 180, 0, 60)
button.Font = Enum.Font.SourceSans
button.Text = "Continue"
button.TextColor3 = Color3.fromRGB(255, 255, 255)
button.TextSize = 39.000
button.TextWrapped = true

-- Script
button.MouseButton1Down:connect(function()
frame:Destroy()
-- you script here ↓

end)
```

# Slider Scripts



# Set Speed Script
```lua
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = val
```


# Set Jump Power Script
```lua
game.Players.LocalPlayer.Character.Humanoid.JumpPower = val
```


# Set Gravity Script
```lua
if val == "" then   
	val = "200"   
	else  
	game.Workspace.Gravity = val  
	end 
```


# Set Fov Script
```lua
if val == "" then
		val = "70"
		end
		game:GetService("Workspace").CurrentCamera.FieldOfView = val -- Set it to the default value (70 is the default FOV)
```

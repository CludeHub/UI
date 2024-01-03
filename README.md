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

# Booting Library
```typescript
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
```
# Make Window
```lua
local Window = OrionLib:MakeWindow({Name = "Title of the library", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})
```
# Tab
```lua
local Tab = Window:MakeTab({
	Name = "Tab 1",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
```
# Notification
```lua
OrionLib:MakeNotification({
	Name = "Title!",
	Content = "Notification content... what will it say??",
	Image = "rbxassetid://4483345998",
	Time = 5
})
```
# Button
```lua
Tab:AddButton({
	Name = "Button!",
	Callback = function()
      		print("button pressed")
  	end    
})
```
# toggle
```lua
Tab:AddToggle({
	Name = "This is a toggle!",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})
```
# Color Picker
```java
Tab:AddColorpicker({
	Name = "Colorpicker",
	Default = Color3.fromRGB(255, 0, 0),
	Callback = function(Value)
		print(Value)
	end	  
})
```
# Slider
```lua
Tab:AddSlider({
	Name = "Slider",
	Min = 0,
	Max = 20,
	Default = 5,
	Color = Color3.fromRGB(255,255,255),
	Increment = 1,
	ValueName = "bananas",
	Callback = function(Value)
		print(Value)
	end    
})
```
 # Label
 ```lua
 Tab:AddLabel("Label")
```
 # Paragraph
 ```lua
Tab:AddParagraph("Paragraph","Paragraph Content")
```
# TextBox
```lua
Tab:AddTextbox({
	Name = "Textbox",
	Default = "default box input",
	TextDisappear = true,
	Callback = function(Value)
		print(Value)
	end	  
})
```
# Keybind
```lua
Tab:AddBind({
	Name = "Bind",
	Default = Enum.KeyCode.E,
	Hold = false,
	Callback = function()
		print("press")
	end    
})
```
# Dropdown
```lua
Tab:AddDropdown({
	Name = "Dropdown",
	Default = "1",
	Options = {"1", "2"},
	Callback = function(Value)
		print(Value)
	end    
})```
# Finishing the Library
```lua
OrionLib:Init()
```
# destroying the interface 
```lua
OrionLib:Destroy()
```


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

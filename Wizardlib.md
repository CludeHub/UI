# Wizard lib
# booting library
```lua

local Library = loadstring(Game:HttpGet("https://raw.githubusercontent.com/bloodball/-back-ups-for-libs/main/wizard"))()
```
# Make Window
```lua
local PhantomForcesWindow = Library:NewWindow("title")
```
# Make tab section
```lua
local KillingCheats = PhantomForcesWindow:NewSection("Kill Options")
```
# make button
```lua
KillingCheats:CreateButton("Button", function()
print("HI")
end)
```
# make textbox
```lua
KillingCheats:CreateTextbox("TextBox", function(text)
        print(text)
end)
```
# Make Toggle 
```lua
KillingCheats:CreateToggle("Auto Ez", function(value)
print(value)
end)
```
# Make Dropdown
```lua
KillingCheats:CreateDropdown("DropDown", {"Hello", "World", "Hello World"}, 2, function(text)
print(text)
end)
```
# Create slider
```lua
KillingCheats:CreateSlider("Slider", 0, 100, 15, false, function(value)
print(value)
 end)
```
# Crete Color picker
```lua
KillingCheats:CreateColorPicker("Picker", Color3.new(255, 255, 255), function(value)
print(value)
end)
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

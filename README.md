# SECRET LIBRARY
never lose

# Booting The Library
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/GhostDuckyy/UI-Libraries/main/Neverlose/source.lua"))()
```


# Creating Window
```lua
local Window = Library:Window({
    text = "Window"
})
```


# Creating Tab
```lua
local TabSection = Window:TabSection({
    text = "TabSection"
})
```

# Creating Section
```lua
local Section = Tab:Section({
    text = "Section"
})
```

# Creating Button
```lua
Section:Button({
    text = "Button",
    callback = function()
        print("Clicked button")
    end,
})
```


# Creating CheckBox Toggle
```lua
Section:Toggle({
    text = "Toggle",
    state = false, -- Default boolean
    callback = function(boolean)
        print("Toggle current: ",boolean)
    end
})
```


# Creating Slider
```lua
Section:Slider({
    text = "Slider",
    min = 10,
    max = 100,
    -- [[Float = 0,]] Idk what it does
    callback = function(number)
        print(number)
    end
})
```

# Creating dropdown
```lua
Section:Dropdown({
    text = "Dropdown",
    list = {"Apple", "Banana","Coconut"},
    default = "Apple",
    callback = function(String)
        print(String)
    end
})
```

# Creating textbox
```lua
Section:Textbox({
    text = "Textbox",
    value = "Default",
    callback = function(String)
        print(String)
    end
})
```

# Creating Color Picker
```lua
Section:Colorpicker({
    text = "Colorpicker",
    color = Color3.new(1,1,1),
    callback = function(HSV)
        print(HSV)
    end
})
```

# Creating KeyBind
```lua
Section:Keybind({
    text = "Keybind",
    default = Enum.KeyCode.Z,
    callback = function(defaultBind)
        print("Triggered keybind")
        print(defaultBind)
    end
})
```

# Slider or Textbox Scripts



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

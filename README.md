# SECRET LIBRARY

# Booting The Library
```lua
local sex = loadstring(game:HttpGet('https://raw.githubusercontent.com/3345-c-a-t-s-u-s/Garry-UI/main/source'))()
```


# Creating Window
local Window = sex:Create('title of the Library','title of game','TEST')



# Creating Tab
local ExampleTab = Window:CreateTab('Tab 1','earth')



# Creating Button
ExampleTab:CreateButton("Button",function()	   
 print('press button')    
end)



# Creating Toggle
ExampleTab:CreateToggle("Toggle",false,function(val)     
	print('toggle',val)     
end)



# Creating Slider
ExampleTab:CreateSlider("Slider",1,100,10,function(val)     
	print('slider',val)     
end)



# Create Label
ExampleTab:CreateLabel("Label")



# Creating KeyBind
ExampleTab:CreateKeybind("Keybind",Enum.KeyCode.E,function(val)     
	print('keybind',val)      
end)



# Creating Window Button Earth
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



# Creating Window Button ADS
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



# Slider Scripts



# Set Speed Script
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = val



# Set Jump Power Script
game.Players.LocalPlayer.Character.Humanoid.JumpPower = val



# Set Gravity Script
if val == "" then   
	val = "200"   
	else  
	game.Workspace.Gravity = val  
	end 



# Set Fov Script
if val == "" then
		val = "70"
		end
		game:GetService("Workspace").CurrentCamera.FieldOfView = val -- Set it to the default value (70 is the default FOV)


# Tora Library
Simple Ui Library. With Clean And Sexy Ui
Note : This Is The Old Version, The Difference Is Font!!!

### Setup The Library
```lua
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/liebertsx/Tora-Library/main/src/library",true))()
```


### Adding Tab
```lua
local tab = library:CreateWindow("Your Title")
```



### Adding Folder
```lua
local folder = tab:AddFolder("Folder")
```



### Adding Button
```lua
folder:AddButton({
	text = "Click me",
	flag = "button",
	callback = function()
	print("hello world")
end
})
```




### Adding Toggle
```lua
folder:AddToggle({
	text = "Toggle",
	flag = "toggle",
	callback = function(v)
	print(v)
end
})
```




### Adding Label
```lua
folder:AddLabel({
	text = "This Is Sick!",
	type = "label"
	})
```





### Adding Slider
```lua
folder:AddSlider({
	text = "Fov",
	min = 70,
	max = 170,
	dual = true,
	type = "slider",
	callback = function(v)
	print(v)
end
})
```





### Adding TextBox
```lua
folder:AddColor({
	text = "Color Picker",
	flag = "color",
	type = "color",
	callback = function(v)
	print(v)
end
})
```





### Adding Dropdown
```lua
folder:AddList({
    text = "Color",
    values = {"Red", "Green", "Blue"},
    callback = function(value)
        print("Selected color:", value)
    end,
    open = false,
    flag = "color_option"
})
```





### Adding Bind
```lua
folder:AddBind({
    text = "bind",
    key = "X",
    hold = false,
    callback = function()
    end
})
```




### Final (REQUIRED OR THE UI WILL NOT SHOW)
```lua
library:Init()
```


### Credits : Tora Is Me

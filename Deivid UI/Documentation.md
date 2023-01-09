# Deivid Library

Documentation for Deivid Library.

## Starting the Library
```
local Library = loadstring(game:HttpGet('https://raw.githubusercontent.com/DeividComSono/Library/main/Deivid%20UI/source.lua'))()
```

## Creating a Window
```
local Window = Library:CreateWindow({
    Name = "Library Name", -- The name of the UI
    SizeX = 450, -- The Size X (Width) of the UI
    SizeY = 300 -- The Size Y (Height) of the UI
})
```

## Creating a Tab
```
local MainTab = Window:CreateTab({
    Name = "Library Name", -- The name of the Tab
    Icon = ""rbxassetid://12060400978" -- The icon of the Tab
})
```

## Creating a Button
```
local Button = MainTab:NewButton({
    Name = "Preview Button", -- The name of the Button
    Callback = function() -- The function after click the Button
        print("Button has been clicked")
    end
})
```

### Uptade Button Name
```
Button:SetText("Name Changed")
```

### Uptade Button Callback
```
Button:SetCallback(function()
    print("Callback Changed")
end)
```

## Creating a Toggle
```
local Toggle = MainTab:NewToggle({
    Name = "Preview Toggle", -- The name of the Toggle
    Default = false, --  The default state of the Toggle
    Callback = function(Value) -- The function after click the Toggle
        print(Value)
    end
})
```

### Uptade Toggle Value
```
Toggle:Set(true)
```

## Creating a Slider
```
local Slider = MainTab:NewSlider({
    Name = "Preview Slider", -- The name of the Slider
    Min = 0, -- The min value of the Slider
    Max = 100, -- The max value of the Slider
    Default = 50, -- The default value of the Slider
    Callback = function(Value) -- The function of the Slider
        print(Value)
    end
})
```

## Creating a Label
```
local Label = MainTab:NewLabel({
    Text = "Preview Label" -- The text of the Label
})
```

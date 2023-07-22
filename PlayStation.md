# PlayStation UI lib 
this is a PlayStation UI lib guide made by ccfe_3

## creating a Gui
```lua
local GUI = loadstring(game:HttpGet("https://raw.githubusercontent.com/bloodball/-back-ups-for-libs/main/aaaa"))()

```

## creating a Ui
```lua
local UI = GUI:CreateWindow("","") -- :CreateWindow(Title,Info) Note: info no space

```

## creating a Tab
```lua
local Tab = UI:addPage("Main",1,true,6) -- :addPage(Title, Scoll Size, Visible, elementspacing)
-- Note: Dont have update function

```

## creating a button
```lua
Tab:addButton('This a button', function() -- :addButton(Title, callback)
    print('Clicked Button')
end)

```

## creating a label
```lua
Tab:addLabel('This a Label', 'Label info') -- :addLabel(Title, Info)
```

## creating a toggle
```lua
Tab:addToggle('Toggle', function(value) -- :addToggle(Title, callback)
    if value then -- if true then
        print('True') -- print true
    else -- else false
        print('False') -- print false
    end
end)
```

## creating a slider
```lua
Tab:addSlider('Slider', 1,100, function(value) -- :addSlider(Title, min, max, callback)
    print(value)
end)
```

## creating a textbox
```lua
Tab:addTextBox('Textbox', 'Textbox Info', function(text) -- :addTextBox(Title, Info)
    print(text)
end)
```

## creating a dropdown
```lua
Tab:addDropdown('This is DropDown', {1', '2', '3', '4', '5'}, 4, function(value) -- :addDropdown(Title, {'List', 'Yeah'}, Scroll Size, callback)
    if value == '1' then
        -- Add script for option 1
    elseif value == '2' then
        -- Add script for option 2
    elseif value == '3' then
        -- Add script for option 3
    elseif value == '4' then
        -- Add script for option 4
    elseif value == '5' then
        -- Add script for option 5
    end
end)

```

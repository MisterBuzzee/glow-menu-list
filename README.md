CSS EDIT

[Original Repo](https://github.com/Glow-Modify/glow-menu-list) 

"Menu in list form, based on esx_menu_list, created for users who don't use the ESX framework. We designed this list due to the decreasing number of ESX framework users." - Glow Modify

TEMPLATE: 
```
	local data = {
		searchEnabled = true, --Search bar.
		title = "Title", --Title on the list.
		columns = {
			{name = "Category 1", width = 25, numChars = 18}, --Column width percentage and the number of characters after which the text is truncated.
			{name = "Category 2", width = 25, numChars = 18},
			{name = "Category 3", width = 25, numChars = 18},
			{name = "Category 4", width = 25, numChars = 18}
		},
		data = {
			{"Long Text Long Text Long Text Long Text Long Text Long Text Long Text Long Text", "Text", "Text", {{text = "Button 1", id = "button1"}}},
			{"Text", "Text", "Text", {{text = "Button 1", id = "button2"}}},
			{"Text", "Text", "Text", {{text = "Button 1", id = "button3"}}},
			{"Text", "Text", "Text", {{text = "Button 1", id = "button4"}}},     
		}
	}
	local Menu = exports['glow-menu-list']:OpenMenuList(data)
	if Menu.ButtonData == 'button1' then
		--Your Code
	end
```

Edit button colors and close icon colors at the top of style.css
```
:root {
    --button-color:   #1864AB;
    --button-hover:   #1971c2;
    --close-color:    #C92A2A;
    --close-hover:    #F03E3E;
}
```
![New Image](https://d1ka0itfguscri.cloudfront.net/ACQn/2024/04/24/11/43/cZfZX5VMoKX/preview.jpg)

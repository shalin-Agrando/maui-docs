---
title: Sticky Group Headers
page_title: .NET MAUI ListView Documentation | Grouping
description: Check our &quot;Sticky Group Headers&quot; documentation article for Telerik ListView for .NET MAUI.
position: 6
slug: listview-sticky-group-header
description: Describing RadListView grouping feature
tags: group, radlistview, groupdescriptor, sticky, group, headers
---

# Sticky Group Headers

RadListView provides the option to set its group headers as sticky. This means the GroupHeader will "freeze" while scrolling through the items until the whole group is scrolled away. As you scroll through the next group, the currently sticked group header will be pushed by the next group header. 

To enable the sticky group headers behavior, just set **IsGroupHeaderSticky** property of the ListView to **True**. By default IsGroupHeaderSticky value is False.

```XAML
<telerikDataControls:RadListView x:Name="listView" 
                                  IsGroupHeaderSticky="True"  />
```
```C#
var listView = new RadListView();
listView.IsGroupHeaderSticky = true;
```

Check below the sticky group headers in action:

![ListView Sticky Group Headers](../images/listview_stickyheaders.gif)

## See Also

- [Filtering]({%slug listview-features-filtering%})
- [Sorting]({%slug listview-features-sorting%})
- [Selection]({%slug listview-features-selection%})
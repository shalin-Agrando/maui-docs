---
title: Selection
page_title: .NET MAUI DatePicker Documentation | Selection
description: Check our &quot;Selection&quot; documentation article for Telerik DatePicker for .NET MAUI.
position: 5
slug: datepicker-selection
---

# Selection

The DatePicker control enables the application users to quickly and easily select a date value by providing an API related to date selection.

## Important Properties

The `Date`(`DateTime?`) proprty defines the current date selection. Its default value is `null`.

The following example demonstrates how to set the `Date` property.

<snippet id='datepicker-keyfeatures-date-spinnerformat' />
```XAML
<telerikInput:RadDatePicker Date="2020,05,15"
                            SpinnerFormat="yyy-MMM"/>
```

In addition to this, you need to add the following namespace:

```XAML
xmlns:telerikInput="clr-namespace:Telerik.XamarinForms.Input;assembly=Telerik.Maui.Controls.Compatibility"
```

## Methods

The DatePicker for .NET MAUI allows you to clear the selected date through its `ClearSelection` method:

```XAML
<StackLayout>
    <Button Text="Clear Selection" Clicked="OnClearSelectionClicked"/>
    <telerikInput:RadDatePicker x:Name="datePicker"/>
</StackLayout>
```

In addition to this, you need to add the following namespace:

```XAML
xmlns:telerikInput="clr-namespace:Telerik.XamarinForms.Input;assembly=Telerik.Maui.Controls.Compatibility"
```

Call `ClearSelection` inside the button `click` event. As a result, the `Date` property will be updated to `null`.

```C#
private void OnClearSelectionClicked(object sender, EventArgs e)
{
    this.datePicker.ClearSelection();
}
```

## Events

The DatePicker exposes a `SelectionChanged` event, which is raised when the user picks a date value.

The following example demonstrates how to use `SelectionChanged`.

```XAML
<telerikInput:RadDatePicker SelectionChanged="RadDatePicker_SelectionChanged"/>
```

In addition to this, you need to add the following namespace:

```XAML
xmlns:telerikInput="clr-namespace:Telerik.XamarinForms.Input;assembly=Telerik.Maui.Controls.Compatibility"
```

Add the `SelectionChanged` event, where the `sender` is the `RadDatePicker` instance.

```C#
private void RadDatePicker_SelectionChanged(object sender, EventArgs e)
{
	// implement your logic here
}
```

## See Also

- [Default Dates]({%slug datepicker-default-dates%})
- [Commands]({% slug datepicker-commands%})
- [Templates]({% slug datepicker-templates%})
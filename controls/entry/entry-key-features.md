---
title: Key Features
page_title: .NET MAUI Entry Documentation | Key Features
description: Check our &quot;Key Features&quot; documentation article for Telerik Entry for .NET MAUI control.
position: 2
slug: entry-key-features
---

# Key Features

The purpose of this help article is to show you the key features of the **RadEntry** control. 

## Text

The following properties are related to the Entry Text appearance and alignment:

* **Text**(*string*): Defines the Text;
* **TextColor**(*Color*): Defines the color of the visible text of the RadEntry control.
* **VerticalTextAlignment**(*of type Xamarin.Forms.Textalignment*): Specifies the vertical alignment of the RadEntry.Text;
* **HorizontalTextAlignment**(*of type Xamarin.Forms.Textalignment*): Specifies the horizontal alignment of the RadEntry.Text;
* **Padding**(*Thickness*): Defines the Padding of the text;

## Watermark 

RadEntry exposes **WatermarkText**(*string*) property used to give guidance to the end user on what should be entered in the text input. The watermark text is displayed when the control is empty.  Additionally, you could set **WatermarkTextColor**(*Color*) to customize the look of the watermark text. 

```XAML
<telerikInput:RadEntry WatermarkText="First Name" WatermarkTextColor="#6EA3FF" />
```

Where:

```XAML
xmlns:telerikInput="clr-namespace:Telerik.XamarinForms.Input;assembly=Telerik.XamarinForms.Input"
```

## Password

RadEntry provides **IsPassword**(*bool*) property, which when set to True, replaces the input with password hint character.

```XAML
<telerikInput:RadEntry IsPassword="True" />
```

## Read-Only State

RadEntry control provides a feature which allows you to choose whether the control will be editable or not - Read-Only state.

* **IsReadOnly** *bool* property: Specifies whether the control will be in edit mode. The default value is `False`. If you want to restrict the control from editing, set the `IsReadOnly` to `True`

```XAML
<telerikInput:RadEntry x:Name="telerikEntry" Text="Telerik UI for Xamarin Entry control" IsReadOnly="True"/>
```

## Max Length

With RadEntry you can restrict the number of the symbols allowed to be entered in the input field. 

* **MaxLength** (*int*) property: Specifies the maximum number of symbols allowed to be entered.

### Example with MaxLength set to 10

```XAML
<telerikInput:RadEntry x:Name="telerikEntry" WatermarkText="Enter text" MaxLength="10" />
```

## Keyboard

The **Keyboard** property of type *Xamarin.Forms.Keyboard* allows you to define the type of the keyboard that will be visualized by the device.

```XAML
<telerikInput:RadEntry x:Name="entry" 
                       Keyboard="Numeric"
                       WatermarkText="Watermark Text" />
```

## Text Selection

The following properties are related to the Entry text selection: 

* **CursorPosition**(*int*) Specifies the starting position of the text selected in the entry.
* **SelectionLength**(*int*) Specifies the number of characters in the current selection in the entry control.

The next snippet shows how both could be applied in order to preselect part of the Text of the Entry when the control receives the focus:

```XAML
<StackLayout Orientation="Horizontal">
    <telerikInput:RadEntry x:Name="selectEntry" Text="select some text" />
    <telerikInput:RadButton Text="Focus" Clicked="FocusButtonClicked" />
</StackLayout>
```

And the Clicked event handler:

```C#
private void FocusButtonClicked(object sender, System.EventArgs e)
{
    selectEntry.Focus();
    selectEntry.CursorPosition = 7;
    selectEntry.SelectionLength = 9;
}
```

Here is the end result:

![Entry Key Features Example](images/entry_key_features.png)

## Font Options:

RadEntry control has the following properties for defining the Font Options:

* **FontAttributes**
* **FontFamily**
* **FontSize**

```XAML
<StackLayout>
    <telerikInput:RadEntry Text="Normal Text" x:Name="entry"/>
    <telerikInput:RadEntry Text="Bold Text - Large" FontAttributes="Bold" FontSize="Large" />
    <telerikInput:RadEntry Text="Italic Text - Medium" FontAttributes="Italic" FontSize="Medium"/>
    <telerikInput:RadEntry Text="Italic and Bold Text - Small"  FontSize="Small" x:Name="smallEntry"/>
    <telerikInput:RadEntry Text="Micro Text"  FontSize="Micro" />
</StackLayout>
```

>tip For a full list of the provided properties of RadEntry, check its API reference here: [RadEntry Properties](https://docs.telerik.com/devtools/xamarin/api/Telerik.XamarinForms.Input.RadEntry.html#properties).

## See Also

- [Events]({% slug entry-events%})
- [Theming and Style]({% slug entry-theming-style%})
- [Getting Started]({% slug entry-getting-started%})
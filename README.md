# Material.Components.Maui

English | [δΈ­ζ](README_zh.md)

Material You Components for .NET MAUI

![](assets/preview.png)



## Getting Started

- Clone this repo and ref it to your maui project
- Add UseMaterialComponents in your "MauiProgram.cs"

```C#
using Material.Components.Maui.Extensions;

namespace SampleApp;
public static class MauiProgram
{
    public static MauiApp CreateMauiApp()
    {
        var builder = MauiApp.CreateBuilder();
        builder
            .UseMauiApp<App>()
            .UseMaterialComponents(new List<string>
            {
                //generally, we needs add 6 types of font families
                "xxx-Regular.ttf",
                "xxx-Italic.ttf",
                "xxx-Medium.ttf",
                "xxx-MediumItalic.ttf",
                "xxx-Bold.ttf",
                "xxx-BoldItalic.ttf",
            });
        return builder.Build();
    }
}
```

- Add Material colors&styles in  your "App.xaml"

```xaml
<?xml version="1.0" encoding="UTF-8" ?>
<Application
    x:Class="SampleApp.App"
    xmlns="http://schemas.microsoft.com/dotnet/2021/maui"
    xmlns:x="http://schemas.microsoft.com/winfx/2009/xaml"
    xmlns:local="clr-namespace:SampleApp"
    xmlns:mds="clr-namespace:Material.Components.Maui.Styles;assembly=Material.Components.Maui">
    <Application.Resources>
        <ResourceDictionary>
            <ResourceDictionary.MergedDictionaries>
                <ResourceDictionary Source="Resources/Styles/Colors.xaml" />
                <ResourceDictionary Source="Resources/Styles/Styles.xaml" />
                <mds:MaterialStyles />
                <!--or use seendColor
                <mds:MaterialStyles Dark="DarkBlue" Light="Green" />-->
            </ResourceDictionary.MergedDictionaries>
        </ResourceDictionary>
    </Application.Resources>
</Application>
```

- Let's go



## The available controls

> π: ready    π€: unverified    π­: needs help

| control   | android    | windows   |  ios&mac   |
| ---- | ---- | ---- |----|
| button    | π | π | π€ |
| IconButton | π | π |π€|
| Card | π | π |π€|
| CheckBox | π | π |π€|
| Chip | π | π |π€|
| ComboBox | π | π |π­|
| ContextMenu | π | π |π­|
| FAB | π | π |π€|
| Label | π | π |π€|
| NavigationBar | π | π |π­|
| NavigationDrawer | π | π |π­|
| Popup | π | π |π­|
| ProgressIndicator | π | π |π€|
| RadioButton | π | π |π€|
| SplitView | π | π |π­|
| Switch | π | π |π€|
| Tabs | π | π |π­|
| WrapLayout | π | π |π€|

## Contributing

Plan on contributing to the repository? We're glad to have you



## License

MIT



## Documentation

TODO






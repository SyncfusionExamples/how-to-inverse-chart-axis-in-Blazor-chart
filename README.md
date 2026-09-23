# How to Inverse the Chart Axis in Syncfusion Blazor Chart

## Overview

This sample demonstrates how to invert the primary X-axis in a Syncfusion [Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts) by using the `IsInversed` property of `ChartPrimaryXAxis`. In a standard chart, category values are rendered from left to right according to their source order. By enabling axis inversion, the categories are displayed in reverse order, which can be useful for comparison scenarios, chronological reversal, or customized business reporting requirements.

The sample renders a column chart using a category axis and a simple collection of weather-report data. The chart visualizes categories for days of the week while displaying the axis in reverse order.

## Key Features

- Uses the `SfChart` component to render chart data.
- Configures `ChartPrimaryXAxis` with:
  - `ValueType="Syncfusion.Blazor.Charts.ValueType.Category"`
  - `IsInversed="true"`
- Uses a `ChartSeriesCollection` containing a `ChartSeries`.
- Binds chart data through:
  - `DataSource`
  - `XName`
  - `YName`
- Renders data as a column chart using:
  - `Type="ChartSeriesType.Column"`
- Demonstrates category-based axis rendering with inverted display order.
- Uses a strongly typed `ChartData` model containing:
  - `string X`
  - `double Y`

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone the repository.
2. Open Visual Studio 2022.
3. Select **Open a project or solution**.
4. Browse to the project file:
 
`InverseChartAxis.csproj`
 
5. Restore NuGet packages if prompted.
6. Build the project.
7. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Clone the repository.
2. Open the repository folder in Visual Studio Code.
3. Open the integrated terminal.
4. Navigate to the project directory containing `InverseChartAxis.csproj`.

```bash
dotnet restore
dotnet run
```

5. Open the local application URL displayed in the terminal output.

## Project Structure

`Pages/Index.razor` - Main sample page containing the `SfChart`, `ChartPrimaryXAxis`, `ChartSeriesCollection`, `ChartSeries`, and sample chart data implementation.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- For official documentation related to HeatMap appearance customization, visit https://help.syncfusion.com/chart-sdk/blazor/charts/axis-customization

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.
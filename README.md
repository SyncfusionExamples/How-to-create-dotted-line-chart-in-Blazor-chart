# How to Create a Dotted Line Chart in Blazor Using Syncfusion Charts

## Overview

This sample demonstrates how to create a dotted or dashed line chart using Syncfusion [Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts). The implementation renders a line series with a custom dash pattern by using the `DashArray` property of `ChartSeries`.

The sample binds a strongly typed collection of data objects to a line chart and displays category-based values across multiple countries. This approach is useful for visualizing trends, forecasts, threshold indicators, or comparison datasets where dashed or dotted lines help distinguish a series from other chart elements.

## Key Features

- Uses the `SfChart` component to render chart data.
- Configures the primary X-axis using `ChartPrimaryXAxis`.
- Sets `ValueType="ValueType.Category"` for category-based axis labels.
- Uses a `ChartSeries` configured with:
  - `Type="ChartSeriesType.Line"`
  - `DataSource` for data binding
  - `XName` and `YName` field mappings
  - `DashArray="5,5"` to render a dashed/dotted line pattern
  - `Width="3"` to control line thickness
  - `Opacity="0.5"` to control series transparency
  - `Fill="blue"` to define the series color
- Demonstrates strongly typed data binding using a custom `ChartData` model.
- Displays line-chart data using category values and corresponding numeric measurements.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open the `DottedLine.csproj` project file.
3. Restore NuGet packages when prompted.
4. Build the project.
5. Run the application using `Ctrl+F5`.
6. Navigate to the page hosting the chart sample to view the dotted line chart.

**Visual Studio Code**

1. Clone or download this repository.
2. Open the repository folder in Visual Studio Code.
3. Open the integrated terminal.
4. Navigate to the project directory.

```bash
cd DottedLine
dotnet restore
dotnet run
```

5. Open the local application URL displayed in the terminal after the application starts.

## Project Structure

`DottedLine/Pages/Index.razor` — Implements the Syncfusion chart sample, data model, category axis configuration, line-series definition, and `DashArray` customization used to render the dotted line.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Official documentation for Syncfusion Blazor Chart: https://help.syncfusion.com/chart-sdk/blazor/charts/getting-started

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.
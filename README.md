# how-to-inverse-chart-axis-in-Blazor-chart

[Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts) provides the support to inverse the chart axis. By setting the [IsInversed](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.ChartCommonAxis.html#Syncfusion_Blazor_Charts_ChartCommonAxis_IsInversed) property to true, you can inverse the axis.

The following code illustrates how to inverse the primary axis(X-Axis).

**C#**

```cshtml

<ChartPrimaryXAxis IsInversed="true" /> 

```

**Index.razor**

```cshtml

@using Syncfusion.Blazor.Charts

<SfChart Title="Weather Reports">
   <ChartPrimaryXAxis ValueType="Syncfusion.Blazor.Charts.ValueType.Category" IsInversed="true" />   

   <ChartSeriesCollection>
       <ChartSeries DataSource="@WeatherReports" XName="X" YName="Y" Type="ChartSeriesType.Column" />
   </ChartSeriesCollection>
</SfChart>

@code{

   public class ChartData
   {
       public string X { get; set; }
       public double Y { get; set; }
   }
   
   public List<ChartData> WeatherReports = new List<ChartData>
   {
       new ChartData { X = "Sun", Y = 35 },
       new ChartData { X = "Mon", Y = 40 },
       new ChartData { X = "Tue", Y = 80 },
       new ChartData { X = "Wed", Y = 70 },
       new ChartData { X = "Thu", Y = 65 },
       new ChartData { X = "Fri", Y = 55 },
       new ChartData { X = "Sat", Y = 50 }
   };
}

```

The following screenshot illustrates the result of the above code snippet.

**Output:**

![](/inverse-axis-in-blazor-chart.png)

**Conclusion**

I hope you enjoyed learning how to inverse the chart axis in Blazor Chart Component.

You can refer to our [Blazor Chart feature tour](https://www.syncfusion.com/blazor-components/blazor-charts) page to know about its other groundbreaking feature representations and [documentation](https://blazor.syncfusion.com/documentation/chart/getting-started), and how to quickly get started for configuration specifications. You can also explore our [Blazor Chart example](https://blazor.syncfusion.com/demos/chart/line?theme=bootstrap5) to understand how to create and manipulate data.
For current customers, you can check out our components from the [License and Downloads](https://www.syncfusion.com/sales/teamlicense) page. If you are new to Syncfusion, you can try our 30-day [free trial](https://www.syncfusion.com/downloads/blazor) to check out our other controls.

If you have any queries or require clarifications, please let us know in the comments section below. You can also contact us through our [support forums](https://www.syncfusion.com/forums), [Direct-Trac](https://support.syncfusion.com/create), or [feedback portal](https://www.syncfusion.com/feedback/blazor-components?control=charts). We are always happy to assist you!

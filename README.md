# Reporting for WPF - Customize the `Choose a Report Color Scheme` Wizard Page

This example shows how to customize the [Choose a Report Color Scheme](https://docs.devexpress.com/XtraReports/400459/create-end-user-reporting-applications/wpf-reporting/end-user-report-designer/gui/report-wizard/table-report/choose-a-report-color-scheme) wizard page in a WPF application.

The main steps to change the color scheme set on the Report Wizard page are as follows:

1. Implement the [IColorSchemeStorage](https://docs.devexpress.com/XtraReports/DevExpress.XtraReports.Wizards.ColorSchemes.IColorSchemeStorage) interface. This is a storage for the custom color schemes.
2. Use the [AddColorScheme](https://docs.devexpress.com/XtraReports/DevExpress.XtraReports.Wizards.ColorSchemes.IColorSchemeStorage.AddColorScheme(DevExpress.XtraReports.Wizards.ColorSchemes.ColorScheme)) method to add custom color schemes to the storage.
3. Add a custom service that implements the [IWizardCustomizationService](https://docs.devexpress.com/XtraReports/DevExpress.XtraReports.Wizards.IWizardCustomizationService)  interface. 
4. Register the custom color scheme storage in the <a href="https://docs.devexpress.com/XtraReports/DevExpress.XtraReports.Wizards.IWizardCustomizationService.CustomizeReportWizard(IWizardCustomization-XtraReportModel-)">CustomizeReportWizard</a> method.
5. Register the wizard customization service in XAML.


![Reporting for WPF - Customize the `Choose a Report Color Scheme` Wizard Page](Images/screenshot.png)

## Files to Review

- [MainWindow.xaml](CS\MainWindow.xaml) (VB: [MainWindow.xaml](VB\MainWindow.xaml))
- [CustomColorSchemeStorage.cs](CS\CustomColorSchemeStorage.cs) (VB: [CustomColorSchemeStorage.vb](VB\CustomColorSchemeStorage.vb))
## Documentation

- [Wizard Customization Overview](https://docs.devexpress.com/XtraReports/118019/wpf-reporting/end-user-report-designer-for-wpf/api-and-customization/wizard-customization-overview)

## More Examples

- [WPF Report Designer - How to register a custom page in the Report Wizard](https://github.com/DevExpress-Examples/Reporting_wpf-report-designer-how-to-register-a-custom-page-in-the-report-wizard-t600080)
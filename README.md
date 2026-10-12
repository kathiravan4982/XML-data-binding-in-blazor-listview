# XML Data Binding in Blazor ListView

## Project Overview
This sample demonstrates how to bind XML data to the Syncfusion [Blazor ListView](https://www.syncfusion.com/blazor-components/blazor-listview) component. The application reads an XML file asynchronously, converts its item elements into a list of data objects, and displays the resulting records in the ListView. This approach enables XML-based data to be presented through a structured, interactive list interface.

## Features
- Uses the Syncfusion Blazor `SfListView` component to display records loaded from an XML file.
- Binds the generated `List<DataModel>` collection through the `DataSource` property.
- Maps the `DataModel.Id` and `DataModel.Text` properties through `ListViewFieldSettings`.
- Defines `DataModel` with the `Id` and `Text` properties required by the ListView field mappings.
- Loads the XML records when the component initializes through `OnInitializedAsync`.
- Calls the asynchronous `GetData` method to read and prepare the XML data.
- Reads the contents of `Pages/XMLFile.xml` with `File.ReadAllTextAsync`.
- Parses the XML content into an `XDocument`.
- Selects each `<item>` element and converts its `<Text>` and `<Id>` values into a `DataModel` object.
- Converts the projected XML records into a list and assigns them to the ListView data source.

## Prerequisites
Ensure the following requirements are met before running this project:
- Visual Studio 2022 or Visual Studio Code
- .NET SDK compatible with Blazor

## Installation

### Clone the Repository
Clone the repository and navigate to the project directory:
```bash
git clone https://github.com/SyncfusionExamples/XML-data-binding-in-blazor-listview.git
```
### Run the Application
**Visual Studio 2022**

1. Open the cloned repository folder.
2. Open the solution file:

   `BlazorApp1.sln`

3. Restore the NuGet packages by rebuilding the solution.
4. Set the startup project to:

   `BlazorApp1`

5. Build the solution.
6. Run the application using `Ctrl+F5`.
7. Open the application URL displayed by Visual Studio after launch.
8. Verify that the XML records are displayed in the Blazor ListView.​‌

**Visual Studio Code**

1. Open the cloned repository folder in Visual Studio Code.
2. Open the integrated terminal.
3. Navigate to the project directory:

```bash
cd XML-data-binding-in-blazor-listview
```

4. Restore the NuGet packages:

```bash
dotnet restore
```

5. Run the project:

```bash
dotnet run
```

6. Open the local URL displayed in the terminal after the application starts.
7. Verify that the XML records are displayed in the Blazor ListView.​‌

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Official documentation: [Blazor ListView data binding documentation](https://blazor.syncfusion.com/documentation/listview/data-binding)

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.
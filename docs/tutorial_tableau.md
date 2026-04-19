# Tableau walk-through

_This walk-through uses the **Cooper Collection Stories** sheet as an example. For the lab, you may instead choose a different sheet or pursue the same question you explored in Excel._

## Dataset
Download the dataset here:  
[Cooper Comics Collection data](https://mikrowelle.github.io/cooper-comics-final/data/Cooper%20Comics%20Reprint%20Metadata.xlsx)

For this exercise, we will begin with the **Cooper Collection Stories** sheet.

## 1. Load the data

1. Open Tableau.
2. In the left sidebar, under **To a File**, click **Microsoft Excel**.
3. Select the Cooper Comics Collection Excel file on your computer.  
![Load Excel file](./images/tableau_load1.png)

4. In the list of sheets, drag **Cooper Collection Stories** to the area labeled **Drag tables here**.  
![Drag Stories sheet into the data source area](./images/tableau_load2.png)

You should now see a preview of the data.  
![Data preview](./images/tableau_load2.5.png)

5. Click **Sheet 1** at the bottom of the window.  
![Go to Sheet 1](./images/tableau_load3.png)

<!-- Instructor note: Keep this section brief. Students mainly need to know how to get from the Excel file to a worksheet where they can build a view. -->

## 2. Get oriented in the worksheet

In **Sheet 1**:

- the left sidebar contains the fields from your dataset
- the center is where Tableau builds the view
- the **Rows** and **Columns** shelves control how the view is organized  
![Worksheet overview](./images/tableau_load4.png)

Tableau separates fields into:
- **Dimensions**: categories such as title or genre
- **Measures**: numeric values Tableau can count, sum, or otherwise aggregate

## 3. Build a simple table

Let’s create a table that shows how many stories of each genre appear in each book.

1. Drag **Title - Book** to **Rows**.
2. Drag **Genre - Story** to **Columns**.
3. Drag **Cooper Collection Stories (Count)** into the center of the view.  
![Build a table of genre counts by book](./images/tableau_view1.gif)

You should now have a table showing the count of stories for each combination of **book title** and **story genre**.

## 4. Create a bar chart

A bar chart is a good next step because it makes differences in count easier to compare.

1. In **Show Me**, choose a **bar chart**.  
![Choose a bar chart in Show Me](./images/tableau_view8.png)

This creates a bar chart using the fields already in the view.  
![Bar chart view](./images/tableau_view9.png)

2. If the chart is hard to read, rearrange the fields on the shelves. This changes whether you see:
   - books grouped within genres, or
   - genres grouped within books  
![Reorder fields to change the view](./images/tableau_view10.gif)

3. To make categories easier to distinguish, drag **Genre - Story** to **Color**.  
![Add color to the bar chart](./images/tableau_view11.gif)

4. If you want numbers on the bars, drag **Cooper Collection Stories (Count)** to **Label**.  
![Add labels to bars](./images/tableau_view13.gif)

## 5. Edit titles and labels

### Change the worksheet title

1. Double-click the title above the view.
2. Enter a more descriptive title.  
![Edit worksheet title](./images/tableau_format1.png)

### Change an axis title

You can edit an axis title in two ways:

1. Double-click the axis title in the chart and edit the text.  
![Edit axis title directly](./images/tableau_format2.png)

2. Or right-click a field name in the data pane and choose **Rename**.  
![Rename a field](./images/tableau_format3.png)

### Change formatting

To adjust font, borders, alignment, and related settings:

1. Go to **Format** in the top menu.
2. Choose the setting you want to edit.
3. Use the formatting pane that opens on the left.  
![Open the Format menu](./images/tableau_format4.png)  
![Formatting pane](./images/tableau_format5.png)

<!-- Instructor note: Students do not need to polish extensively. A descriptive title, readable labels, and a sensible chart type are enough. -->

## 6. Optional: try another chart type

If you want to explore further, you can try a different view of the same data.

### Heat map
A heat map can make higher and lower values stand out more clearly.  
![Show Me panel](./images/tableau_view6.png)  
![Heat map option](./images/tableau_view7.png)

### Marks-based view
You can also drag **Cooper Collection Stories (Count)** to **Size** and **Genre - Story** to **Color** to create a marks-based view.  
![Use Size to show larger and smaller counts](./images/tableau_view2.gif)  
![Adjust mark type or size](./images/tableau_view3.gif)  
![Add color by genre](./images/tableau_view4.png)  
![Colored marks view](./images/tableau_view5.png)

A stacked bar chart is another alternative.  
![Stacked bar chart example](./images/tableau_view12.png)

## 7. Optional: duplicate a sheet

If you want to keep one version of your chart and make a second version without starting over:

1. Right-click the **Sheet 1** tab.
2. Choose **Duplicate**.  
![Duplicate a worksheet](./images/tableau_dup1.png)

You can now modify the duplicate while keeping the original.

## 8. Optional: join two sheets

Use this only if you want to combine information from different sheets.

For example, the **Stories** sheet includes story-level information, while the **Books** sheet includes book-level information such as publisher.

1. Go back to the **Data Source** tab.
2. Drag **Cooper Collection Books** into the top area with **Cooper Collection Stories**.  
![Add a second sheet in Data Source](./images/tableau_join1.png)

3. Tableau will ask how the two sheets relate.
4. Set the matching field in both sheets to **#**.  
![Relate the sheets using #](./images/tableau_join2.png)

5. Return to your worksheet. Tableau now shows fields from both sheets in the data pane.  
![Fields from both sheets now available](./images/tableau_join3.png)

This lets you create views that combine story genre with publisher or other book-level fields.

## 9. What you should have

By the end of this exercise, you should have:
- one Tableau worksheet built from the Cooper data
- one readable visualization
- a title and labels that make the chart understandable

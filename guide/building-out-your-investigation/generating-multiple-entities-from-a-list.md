---
description: >-
  Follow the steps below to extract structured entities from an uploaded
  spreadsheet within an investigation.
---

# Generating multiple entities from a spreadsheet or CSV

## Structuring your data

When **importing a list of companies, people or similar data objects**, it is helpful to convert your raw data into [structured entities](../../developers/followthemoney/) that Aleph can use to classify those entities for searching, cross-referencing, and many other operations.

{% hint style="info" %}
For small and mid-size datasets, follow the instructions below to map your data into structured entities using the Aleph mapping editor. To map very large data straight from a SQL database, or to map complicated relationships, you will have to [create a mapping file](../../developers/mappings.md) instead.
{% endhint %}

### Using the Aleph mapping editor

1. Follow the "Importing documents and files" steps above to **import your .csv, .xls, or .xlsx data file** to an investigation.
2. Once the data file has finished uploading, browse to one of the tables you have uploaded. C**lick the "Generate Entities" tab** to open the mapping editor.

![](../../.gitbook/assets/screenshot-2019-12-02-at-15.32.13.png)

1. **Select the types** of entities you would like to create from your data

![](../../.gitbook/assets/screenshot-2019-12-02-at-15.54.27.png)

1. **Define any relationships** - such as ownership or family relations - that exist between the entities.

![](../../.gitbook/assets/screenshot-2019-12-02-at-16.12.25.png)

1. **Select columns from your data to use as unique keys** for each entity\*\*.\*\*

Keys are usually ID numbers, email addresses, telephone numbers, or other properties of your data which are guaranteed to be unique. The more columns you are able to select as keys, the better, to ensure that Aleph correctly generates an entity for each unique entry in your data.

![](../../.gitbook/assets/screenshot-2019-12-02-at-16.08.29.png)

1. **Assign data columns to properties** of the entity types you have selected.

![](../../.gitbook/assets/screenshot-2019-12-02-at-15.56.15.png)

1. **Add any fixed values to the entities.** If, for instance, your data is a company registry from Moldova, it would be useful to set the "Country" property to "Moldova", so that all company entities that are generated will automatically have their country set as Moldova.

![](../../.gitbook/assets/screenshot-2019-12-02-at-15.57.57.png)

1. **Select an optional destination for the entities that are created**. By selecting a diagram or list here, the entities that are generated from your spreadsheet will be automatically added to that diagram or list, in addition to the investigation of which they are a part.

![](<../../.gitbook/assets/screen-shot-2021-02-11-at-13.16.17 (1).png>)

**9. Verify and submit your mapping**

{% hint style="info" %}
When a mapping is submitted, Aleph will automatically generate structured entities based on the instructions you have provided it. It is important to note that **any** **future edits you make to the mapping will re-generate these entities.** Additionally, deleting the mapping will delete any entities generated from it.
{% endhint %}

1. **After the entity generation process has finished, you should see your entities in the** [**entities view**](using-the-table-editor.md) **of your investigation.**

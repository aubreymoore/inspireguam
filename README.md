# inspireguam

Useful reference: [NYU Libraries/Research Guides/Research Data Management/Storage & Backup](https://guides.nyu.edu/data_management/storage-backup)

Note: It might be possible to automate backups using PyAutoGui.

## Manual Backup
1. Open local copy of Zotero.
1. In the left-hand panel, select **inspireguam**
1. On the main menu, select **File | Export library ...**
1. In the **Export ...** dialog, select **Zotero RDF** as the format.
1. In the **Export ...** dialog, select **Export Notes**, **Export Files**, and **Include Annotations**
1. In the **Export ...** dialog, click the **OK** button
1. Use the **Save** dialog, to save the export to **/home/aubrey/Desktop/inspireguam/backup**

At this point the folder **inspireguam/backup** should contain 2 objects:
* **inspireguam.rdf** which is an XML file containing all of the bibliographic metadata
* **files** which is a folder containing PDFs and possibly other files

Now push to GitHub as usual.

## Restore from Backup
1. If necessary, clone the **inspireguam** repo.
1. Open local copy of Zotero.
1. Create a group library.
1. Select the new group library.
1. On the Zotero main menu select **File | Import ...**
1. Use the **Import** dialog to select **backup.rdf** in the repo


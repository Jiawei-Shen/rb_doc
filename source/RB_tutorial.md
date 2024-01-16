[comment]: <> (# Use the Repeat Browser)

[comment]: <> (Instruction on how to navigate [WashU Repetitive Element Browser]&#40;https://repeatbrowser.org/&#41;)

[comment]: <> (<br />)

[comment]: <> (<br /> )

# Main Page
## The Top Menu
![The Top Bar Menu](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/headbar.jpg)  
The top navigation menu (above) controls the three main parts of Repeat Browser functionality. From the left to right are the Homepage, Input Data, and Data Visualization. You can also get access to documentation and the links to Wang Lab and WashU Med.
## The Tabs
![The Logo of Repeat Browser](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/homepage_RBlogo.jpg) <br />
On the very left is our logo of repeat browser.
## Homepage
![The Tabs of Homepage](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/homepage_homepageTab.jpg) <br />
Click this tab, you will jump to the homepage with some brief introduction.
![The Tabs of Input Data](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/homepage_dataInput.jpg) <br />
This tabs listed the number of current selected files and repeats. Click this tab, you will jump to the data selection section with 4 different selectable pages on the left bar.
![The Tabs of Data Visualization](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/homepage_dataVisualization.jpg) <br />
Click this tab, you will jump to the data visualization section with 3 different selectable pages on the left bar.


## Homepage
![Home Page](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/homepage_main.png) <br />
You can start exploring WashU Repeat Browser from the Homepage (above). There are some brief text and figure illustrations.  

### Github Link
The **Github repo** link provides the raw codes of this web based tool. 

### The two Buttons
The **Start Browsing** button will lead to **Input Data** page to start browsing.

![Tour Window](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/homepage_tourwindow.jpg) <br />
The **Start Guide Tour** button is a tour guide with a tour window as above to introduce our entire site.
For those accessing our site for the first time, we highly recommend trying this button. 
<br />

# Input Data
![Tour Window](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_4pages.jpg) <br />
Input Data page is the first step of utilizing the repeat browser. You can pick the interested data and repeat subfamilies in this tab. On the left, there is four different pages.

## Data and Repeats Display
### The Display Windows
![The Display Windows](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page1.jpg) <br />
On the first page, you will see the selected data and its repeats. Default data, along with repeats, is provided for first-time users. To remove the data or repeats, you can click either the close button or the "remove all" button.
### Session File
![Session File Button](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page1SessionFile.jpg) <br />
Click this button, users can download the session files which containing all the selected data and repeats. Users can restore the repeat browser by uploading this session file. 
### The Format of Session File
![Session File Format](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_sessionFormat.jpg) <br />
The session file is a JSON file that includes data and repeats, as illustrated above. An example is provided below.
```json
{
  "data": [    
    {
      "Assay": "Histone ChIP-seq",
      "Biosample": "liver",
      "Control": "unknown",
      "Mode": "Experiment",
      "Organism": "mm10",
      "Tissue": "unknown",
      "Target": "H3K4me1",
      "id": "ENCFF007KSG",
      "Zarr": "https://s3-obs1.htcf.wustl.edu/repeatbrowser/mm10/chip-seq/histone/Processed_ENCFF007KSG_signal/ENCFF007KSG_signal.zarr/",
      "_id": 1
    }],
  "repeats": [
    {
      "size": 1,
      "name": "HERVK-int",
      "family": "ERVK",
      "class": "LTR"
    }
  ]
}
```

## Files Selection
![Files Selection](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page2.png) <br/>
Pre-processed public datasets can be achieved at this page, the datasets are categorised by Assay and Species (above). You can also check the selected files or start the hands-on tour through the right panel of this page. Lastly, the default files and repeats can also be reset by the button below.<br/>
Detailed files information can be further explored by clicking the numbers to call the form below. 
The information of datasets, including ID, Assasy, Biosample Type, Experiment ID, Organism, and Status, can be explored. The green and red colors of Status column represent available and selected respectively. Users can simply click the status button to select the data. 
To find the data they are interested in, users can utilize the search bar located in the top right corner of the page.
### Basic Table
![The Overview Table](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page2basicTable.png) <br/>
This is an overview table of all the data. Users can click the blue button in the red box to jump into the detailed data table.

### Detailed Data Table
![The Detailed Table](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page2detailedTable.png) <br/>
In this table, users can click the green button to select the data. You can use the search bar on the top right to find your interested data. 
### Reset Button
![The Reset Button](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page2resetButton.png) <br/>
Recall that there is a default setting for the users who first time visit this website. Clicking this button can reset the data to the default data.
### Selected Data Table
![The Selected Data Table](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page2selectedTable.png) <br/>
The data briefly displays some information of the selected data. The "Detailed Tour" button provides a tour guide.


## Upload
![Files Uploading Page](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page3.png) <br/>
Uploading page provides two functions, **Upload Session Json** and **Zarr File URL**, for users to upload their own data or restore the repeat browser.<br/>
You can upload the JSON session file that is downloaded or shared to achieve quick exploration between collaborators.<br/>
You can also upload the personalized Zarr file generated by our [data processing pipeline](https://github.com/Jiawei-Shen/Repeat-Browser) (detailed information can be checked via this link)

### Upload Session Json File
![Session Json File Uploading](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page3uploadSession.png) <br/>
For the **Upload Session Json**, the session Json can be obtained from Selected Data site. You can click to choose the session file to upload or drag and drop. After determine the session file, click the upload button. <br/>
### Upload Zarr File
![Zarr File Uploading](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page3ZarrUpload.png) <br/>
For the **Zarr File URL**, users can utilize our pipeline to create their our zarr file. And input the Zarr url to the link. <br/>
Important note: The Zarr File must be in an online version; only the URL is functional, and local paths will not work.
#### Create a URL with Local Path
For those who run our pipeline with local devices, we provide a method to upload the local Zarr file with URL. <br />


**Step one**, install [http-server](https://www.npmjs.com/package/http-server).
```commandline
brew install http-server
```
For those who has the npm packages,
```commandline
npm install http-server
```
**Step two**, change the path to where your Zarr files located. 
```commandline
cd /path/to/Zarr/
```

**Step three**, run the http-server commands.
```commandline
http-server --cors
```
if your default port is occupied, try these parameters.
```commandline
http-server --cors -p 8081 -a 127.0.0.1
```

**Step Four**, copy the link on the setting port and input it to the Zarr File URL. Here's an example:
![http-server Sample](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_http-serverSample.jpg) <br />

### Create Zarr File
![Create Zarr File](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page3createZarr.png) <br />
We offer an open-source pipeline for users to generate the Zarr file. Feel free to click on the blue link or the GitHub icon to visit the GitHub repository and explore it!
The detailed illustration is provided in the Github repo. 


## Repeats Selection
![Repeats Selection](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page4.png) <br />
The Repeats page (above) features a sunburst plot for convenient selection of repeats at the class, family, and subfamily levels. Users can utilize the **Repeats Search** bar to locate a specific transposable element (TE) subfamily.
On the left is a window to display the selected repeats and a brief introduction.

![Sunburst Plot](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/sunburst_demo.gif) <br />
For this sunburst chart, the inner ring represents "Class" hierarchy and the outer ring represents "Family" hierarchy. <br/>
**Click Once**: Click the outer ring once, Zoom in to the "Subfamily" hierarchy. <br/>
**Click twice**: Click twice to select the repeats and back to the default view. <br/>
**Click the white space in the middle once**: Zoom out to the previous class. <br/>
Sunburst plot can be played with via the GIF demo below. <br/>

![Repeats Search Bar](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/input_page4searchBar.jpg) <br />
Click the repeat in the drop-down list, the clicked repeat will be added.

<br />
<br /> 


![Consensus_Demo](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/Consensus_demo.gif) <br />
**Single click** on the panel would lead to downstream level (class to family to subfamily), and the first **double click** on the panel will select specific family, or subfamily, in which case the colorful panel would become gray. The second **double click** on the panel would undo the selction operation which would lead the panel to colorful one. In contrast, the **single click** on the central white region would back to the upstream level, while the **double click** on the central white region would back to the class level by default.
![Repeats_Selection_Sunburnt](https://wang.wustl.edu/img/repeats_selection_sunburnt.gif)<br/>
Our website includes a useful search feature that allows users to quickly find and select their desired subfamily. By simply typing the name of the subfamily in the search bar and clicking on the corresponding item in the dropdown menu, the subfamily will be selected.


<br />
<br /> 

# Data Visualization
![Data Visualization](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual.png) <br />
Data Visualization Tab is the main function of WashU Repeat Browser. It contains three pages in this tab.

## Heatmap View
![Heatmap View](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/DataVisual_Heatmap.png) <br />
Heatmap View (above) is the first plot embedded in WashU Repeat Browser. It provides the functions where users can cluster columns(repeats) or rows(datasets), or both, as well as re-order the heatmap by any of the methods, alphabetic order, rank by sum, or rank by variance. You can also set the opacity and the number of rows you want to show by the side bar. The different colors at the edge of the matrix denote the different class/family (for the column) and different datasets (for the row).<br/>

### Data Display
![Heatmap Data Display](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page1dataDisplay.png) <br />
In this window, we provide a brief view of selected data in heatmap.

### Function Bar of Heatmap
![Heatmap Function Bar](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page1dataDisplay.png) <br />
This function bar contains several functions for the heatmap. 

### Function Icons
![Heatmap Function Icons](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page1functionIcons.png) <br />
These four icons provides four different functions. <br />
1. Share the weblink. <br />
2. Screenshot. <br />
3. Download the heatmap matrix. <br />
4. Crop the matrix into a smaller heatmap. <br />

### Heatmap Rank Order
![Heatmap Rank](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page1Rank.png) <br />
We provide four different rank order to display the heatmap.

### Heatmap Slider Bar
![Heatmap Slider Bar](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page1sliderBar.png) <br />
We provide some slider bars to customize your parameters of the heatmap. Additionally, there's a search bar tp search the data.

### A Simple Demo
![Heatmap_Demo](https://wang.wustl.edu/img/Heatmap_demo.gif) <br/>


## Consensus View
![Consensus View](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page2.png) <br />

### Ruler Track
![Ruler Track](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page2rulerDemo.gif) <br />
Dragging this ruler, you can change the area of the consensus view displayed.

### Base-Pair Track
![Base-Pair Track](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page2basepair.png) <br />
This base pair track displays the base pair in the consensus region. It won't show the character unless the region is less than 50 base pairs. 

### Main Tracks of Consensus View
![Main Tracks](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page2mainTracks.png) <br />
These three tracks are <br />
1. Genome Coverage. It is the count of genome copies on each base pairs of consensus region. 2, 3. The count of the reads on the consensus region. <br />
2,3. The Read Counts. It is the key tracks. It provides the read counts in user selected data on the consensus region. 
For the ChIP-seq data, it has two tracks (signal and control). For the others sequencing data, it will only have one track (signal).

### Add Tracks Button
![Add Tracks](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page2addTrack.png) <br />
Users may want to add some more tracks of the other data. The figure shows the panel. 

## Genome View
![Genome View Page](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page3genomeviewPage.png) <br />
Genome view (above) is a bird’s eye view of different locations of TE copies on the genome. A filter sets the threshold of enrichment scores of corresponding TE copies is provided.

### Genome Chart
![Genome View](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page3genomeView.png) <br />
This is genome view, each bar in the chromosome is a genome copy. The color corresponds to the RPKM value, with deeper colors indicating higher RPKM values.

### Genome Plot Chart
![Genome View](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page3genomePlot.png) <br />
Regarding the chromosome, we provide a dot plot for a detailed view. To access the plot, simply click on the blue section of the chromosome bar. 

### Link to WashU Genome Browser Panel
![Alert Window](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page3Jump.jpg) <br />
Click the dot in the genome plot, and you can jump to the WashU genome browser. Click Ok in this alert window. <br />
![WashU Genome Browser](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/WashU-Epigenome-Browser.png) <br />

### Filter Bar
![Filter Bar](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page4filterBar.png) <br />
If you wish to filter genome copies on the chromosome, you can utilize the filter bar. This tool can exclude genome copies that are below the specified threshold.

### Genome View Cart
![Filter Bar](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/rb_screenshots/visual_page4filterBar.png) <br />
You have the option to add additional data to the cart. The contents of the cart will then be displayed on the genome view. <br />
And here is the panel to add data.
![Data Panel](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documenttation/rb_screenshots/visual_page3addPanel.png) <br />



You can also switch to the CAGE-seq heatmap through the Assay Type drop down list.<br/>
Heatmap view of enrichment scores of datasets on TE subfamilies. Users can click a specific cell where each cell denotes ratio of average score or RPKM as per below. 
![Heatmap RPKM Calculation](https://wangftp.wustl.edu/~scheng/repeat_browser/documentation/Heatmap_RPKM.png)


## Consensus View
![Heatmap_Jumpto_Consensus](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/Heatmap_jumpto_Consensus.gif)<br/>
Users can click a specific cell and jump to the Consensus View panel.

![Consensus View](https://wangftp.wustl.edu/~scheng/repeat_browser/documentation/DataVisual_ConsensusVIew.png)
Consensus View panel (above) displays epigenomic data anchored on a TE consensus sequence. Both unique reads and multi-reads can be displayed.<br/>

You can explore different biological meanings with different assay types, like open chromatin regions with ATAC-seq data, gene expression level with CAGE-seq, and TF binding sites with ChIP-seq data. The specific TE subfamily on different datasets can also be compared through the **Add Track** function, and the All reads and Uniquely-mapped reads can also be explored. Besides, the genome coverage and raw consensus sequence are also provided for further exploration.
![Consensus_Demo](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/Consensus_demo.gif)<br/>

## Genome View
![Consensus_jumpto_Genome](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/Consensus_jumpto_Genome.gif)<br/>
:bangbang:Users can click the **Genome View** on the left panel or the right-buttom button to jump to the Genome View panel.

![Genome View](https://wangftp.wustl.edu/~scheng/repeat_browser/documentation/DataVisual_GenomeView.png)
Genome view (above) is a bird’s eye view of different locations of TE copies on the genome. A filter sets the threshold of enrichment scores of corresponding TE copies is provided.

You can get the distribution of the uniquely-mapped reads of specific TE subfamily on Genome View and different shades represent different RPKM values (the darker the higher), where you adjust the threshold via the side bar to only show selected reads. The specific TE subfamily on different datasets can also be compared through the **Add Genome Copies** function, where you can explore the expression differences among different datasets.
![Genomeview_Demo](https://s3-obs1.htcf.wustl.edu/repeatbrowser/documentation/Genomeview_demo.gif)<br/>

Furthermore, to enhance the utility of Repeat Browser, we also link the Repeat Browser with WashU Epigenome Browser where users can choose view the interested individual TE copies on the WashU Epigenome Browser, using the **Region set View** function by which we can display multiple genomic locations side by side,optionally with customizable upstream and  downstream flanking regions (below).
![Region View Set](https://wangftp.wustl.edu/~scheng/repeat_browser/documentation/HeLa-S3_STAT1_MER41B_region_view_set.png)





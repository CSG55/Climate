# Climate

This project collects Canadian raw climate data using Environment Canada's datasets for 2016. 


## Prerequisites

This program was created using Java through the Eclipse IDE. In order to set this up on your computer, I recommend you install Eclipse Oxygen. The latest version can be downloaded on this link:
https://www.eclipse.org/downloads/download.php?file=/oomph/epp/oxygen/R2/eclipse-inst-win64.exe

### Setup

Method 1: Setting up as a Git Repository for Eclipse
```
1. Using Eclipse, Hover over File, then click Import.

2. Maximize the Git folder, then select "Projects from Git". Click Next.

3. Click on the bubble that states: "Select archive file:"

4. Select "Clone URl"

5. Where it says 'URl:', paste the following URL: 
https://github.com/CSG55/Climate

6. Click Next, and ensure 'master' is checked. Click Next again.

7. Decide which file location you wish to set the repository in, then click Next. 

8. Make sure "Import existing Eclipse projects" is checked, then click Next.  

6. Click Finish. Your remote repository is now set up, and Eclipse is configured to use it.

```


Method 2: Importing as an "Existing Project"
```
1. Using Eclipse, Hover over File, then click Import.

2. Maximize the General folder, then select "Existing Projects into Workspace". Click Next.

3. Click on the bubble that states: "Select archive file:"

4. Click Browse, then find the zip repo you installed.

5. Select the Project that appears below.

6. Click Finish. The project should now be imported.

```


## Test Cases

In the main function of ClimateGetter.java, specify the climate data for an arbitrary number of cities you wish to search for. The format is CITY,PROVINCE. For example, to look for Hamilton, Ontario, you would enter "HAMILTON,ON". Capitalization does not matter. The current test case is as follows:

```
String[] x = { "Woodstock,on", "Orangeville,ON", "Oakville,ON", "Richmond,BC", "Vancouver,BC", "OTTAWA,ON", "Toronto,ON", "Irvine,AB", "Barrie,ON", "Hamilton,ON" };

```

For any test cases where no city of that provided name and province is found, null is returned. If a city is found but some data is missing for that city, the missing data is represented by a null. 
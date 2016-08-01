# xploredowload
comand-line util to download and rename ieeexplore papers

# Usage

Use the [ieeexplore website](http://ieeexplore.ieee.org/Xplore/home.jsp) to search the paper you want to read.

Find the `paper-number` on the URL, it is the value after the key `arnumber=`, for example:

A valid ieeexplore paper URL is like:
```
ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=5534753
```
In this example the paper number is `5534753`, use this value as argument for ieeexplore comand in linux shell, as follows:

```
./ieeexplore 5534753
```

The script will download the paper (if you have access) and name it as follows:

```
Author-Name_Year_Complete-Paper-Title.pdf
```

# Expected Output

```
:: Downloading Paper Info Please wait ::

:: The folowing paper will be downloaded ::
         TITLE: Translating default theories to normal default theories
         AUTHORS: Yu Sun; Tianwei Xu; Zhiping Li
         YEAR: 2010

./Yu-Sun_2010_Translating-default-theories     [         <=>                                                                           ] 103.24K  50.2KB/s    in 2.1s    

:: The folowing paper have been downloaded ::
         Yu-Sun_2010_Translating-default-theories-to-normal-default-theories.pdf
```



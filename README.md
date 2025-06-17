# AutoCellCounting_test

基于显微图像的PyTorch+CNN自动细胞计数方法
"""

训练数据集: BBBC005 (包含从显微镜图像中分割的细胞核)

数据来源: BBBC (Broad Bioimage Benchmark Collection)

URL: BBBC (https://bbbc.broadinstitute.org/BBBC005)

Introduction: 

    Images：
        Simulated HCS images were generated with the SIMCEP simulating platform for fluorescent cell population images (Lehmussola et al., IEEE T. Med. Imaging, 2007 and Lehmussola et al., P. IEEE, 2008). These images were simulated for a given cell count with a clustering probability of 25% and a CCD noise variance of 0.0001. Focus blur was simulated by applying Gaussian filters to the images. Each image is 696 x 520 pixels in 8-bit TIF format, with the nuclei and cell areas were matched to the average nuclei and cell areas from the BBBC006 (Human U2OS cells (out of focus)) image set.

    The image nomenclature was chosen to permit metadata to be organized in a plate layout. Each image follows the form

        SIMCEPImages_well_Ccells_Fblur;_ssamples_wstain.TIF

    where the variables are as follows:

        well: The standard 384-well plate format is used where the rows are named A-P and the columns 1- 24.

        cells: The number of cells simulated in the image (1-100).

        blur: The amount of focus blur applied (1-48). The focus blur was simulated by using MATLAB's imfilter function with a rotationally symmetric Gaussian lowpass filter of diameter  and sigma of 0.25 × 

        sample: Number of samples (1-25) for a given combination of  and . Can be used to mimic the "site" number for each well.

        stain: 1 = cell body stain, 2 = nuclei stain.

        The result of this plate nomenclature is that "row" represents a given amount of blur and the "columns" are a given cell count.

    There are 19,200 image files.

"""

# GEFSV12 - Primarily for working with GEFS reforecast data on AWS
#GEFS Reforecast data https://registry.opendata.aws/noaa-gefs-reforecast/

#GEFS live FORECAST data https://registry.opendata.aws/noaa-gefs/

Example of listing subdirectory in S3 hosting GEFS reforecast data aws s3 ls s3://noaa-gefs-retrospective/GEFSv12/reforecast/2000/2000123100/c00/Days:1-10/ --no-sign-request

Here are vars to download: gust_sfc_2000123100_c00.grib2 pres_msl_2000123100_c00.grib2 pres_sfc_2000123100_c00.grib2 ugrd_hgt_2000123100_c00.grib2 #vars fixed at 10m and 100 m AGL vgrd_hgt_2000123100_c00.grib2 #vars fixed at 10m and 100 m AGL

aws s3 cp s3://noaa-gefs-retrospective/GEFSv12/reforecast/2000/2000123100/c00/Days:1-10/gust_sfc_2000123100_c00.grib2 --no-sign-request ./ aws s3 cp s3://noaa-gefs-retrospective/GEFSv12/reforecast/2000/2000123100/c00/Days:1-10/pres_msl_2000123100_c00.grib2 --no-sign-request ./ aws s3 cp s3://noaa-gefs-retrospective/GEFSv12/reforecast/2000/2000123100/c00/Days:1-10/pres_sfc_2000123100_c00.grib2 --no-sign-request ./ aws s3 cp s3://noaa-gefs-retrospective/GEFSv12/reforecast/2000/2000123100/c00/Days:1-10/ugrd_hgt_2000123100_c00.grib2 --no-sign-request ./ aws s3 cp s3://noaa-gefs-retrospective/GEFSv12/reforecast/2000/2000123100/c00/Days:1-10/vgrd_hgt_2000123100_c00.grib2 --no-sign-request ./

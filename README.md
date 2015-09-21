# write-EXIF-GPS
Upload GPS coordinates and focal length from UAV log into photos' EXIF.
Input is a CSV file created from a jxl file using [jxl2csv](https://github.com/wenzeslaus/jxl2csv) tool.
The CSV file looks like this:

    name,latitude,longitude,height,yaw,pitch,roll
    DSC01505.JPG,35.72515912,-78.69455195,183.10,-0.024451,0.0474495,-0.0796704
    DSC01506.JPG,35.72535282,-78.69453640,181.82,-0.0341963,-0.0453087,-0.0160694
    DSC01507.JPG,35.72557271,-78.69451902,180.93,0.025517,0.00329905,-0.0783194
    DSC01508.JPG,35.72575487,-78.69450289,181.77,0.0673514,0.0334387,-0.137099
    DSC01509.JPG,35.72599511,-78.69447896,182.18,0.0547578,-0.0137402,-0.0966732
    DSC01510.JPG,35.72620886,-78.69445576,182.60,0.0866429,0.0138617,-0.0725457
    DSC01511.JPG,35.72640986,-78.69443359,182.94,0.0342202,0.0474153,-0.104997
    DSC01512.JPG,35.72661482,-78.69441034,183.25,0.0671639,0.0174592,-0.081061
    DSC01513.JPG,35.72683582,-78.69438373,183.56,0.0761532,-0.00724168,-0.10356

# Usage
pyhton write_EXIF_GPS.py log.csv

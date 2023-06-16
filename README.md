# COCO JSON to YOLO TXT Converter

This script converts COCO JSON annotations into YOLO TXT format for object detection tasks. It reads a COCO JSON file containing annotations for multiple images and outputs YOLO TXT files for each image.

## Prerequisites

- Python 3.x
- `tqdm` library (install using `pip install tqdm`)

## Usage

1. Ensure that the COCO JSON file and the script file are in the same directory.
2. Open the script file and update the following variables if needed:
   - `output_path`: The path where the output files will be saved. The default is `"output"`.
   - `json_file`: The name of the COCO JSON file. Replace `"output_coco.json"` with your own file name if different.

# Example usage
convert_coco_json_to_yolo_txt("output", "output_coco.json")
```

Make sure to replace `"output_coco.json"` with the actual name of your COCO JSON file.

The script will create an output

 folder (if it doesn't exist) and generate the following files inside it:

- `_darknet.labels`: A file containing the names of all classes, with each class on a new line.
- Individual TXT files for each image, containing the annotations in YOLO format.

After running the script, you will find the converted YOLO TXT files in the specified output folder.

Note: This script assumes that the COCO JSON file follows the standard COCO annotation format. Please ensure that the JSON file is formatted correctly before running the script.

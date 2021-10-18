## Description

Given an input file `input/visits-x.jsonl` (in jsonlines format), write a program to create a heat map of the vehicles. After running the program, you should have `output/visits-x.png` with the vehicle rectangles. The most visited location should be white. Areas without any vehicles are black. The intensity of each pixel depends on how many rectangles are drawn on it (see example below).

- Your solution will be judged based on readability, correctness and concision.
- This task should not take more than 1 hour.
- If you complete the exercise quickly, programmatically draw a line representing the average vehicle direction.

## Example And Submission

The file `input/visits-1.jsonl` has 2 vehicles with bounding boxes `{"xmin": 85, "ymin": 98, "xmax": 316, "ymax": 212}` and `{"xmin": 228, "ymin": 160, "xmax": 459, "ymax": 283}`. The file `output/visits-1.png` is gray for each of those rectangles and white where they overlap. There is another example for visits-2.

We will run your script using the following command:

```shell
cd /path/to/exercise
docker build -t exercise .
docker run -v /path/to/exercise:/app exercise
ls output
# Expected output: visits-1.png visits-2.png visits-3.png
```

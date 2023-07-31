# Dataset

* Contains 600 stereo images (150 unregistered left, 150 unregistered right, 150 registered left, 150 registered right)
* The data set contain images of 10 volunteers
* There are 60 images peer volunteer (15 unregistered left, 15 unregistered right, 15 registered left, 15 registered right)

## Dataset structure

### dataset.csv

#### Columns
| column name     | dataype     | description                                                  |
|-----------------|-------------|--------------------------------------------------------------|
| timestamp       | string      | timestamp for the measurement format="%Y-%m-%d__%H:%M:%S.%f" |
| GT_depth        | float       | distance from the cameras to the person in cm                |
| CAL_height      | float       | height calculated by our solution in cm                      |
| person_id       | int         | unique id given to each person in the dataset                |
| GT_hetight      | double      | ground truth height for each person                          |
| GT_hetight      | double      | ground truth height for each person                          |
| unreg_img_left  | string      | path to unregistered left image                              |
| unreg_img_right | string      | path to unregistered right image                             |
| reg_img_left    | string      | path to registered left image                                |
| reg_img_right   | string      | path to registered right image                               |
| error           | float       | absolute error between CAL_height and GT_height              |
| left_1          | float float | relative coordinates of eye 1 in left image                  |
| left_2          | float float | relative coordinates of eye 2 in left image                  |
| left_3          | float float | relative coordinates of mouth in left image                  |
| left_4          | float float | relative coordinates of nose in left image                   |
| right_1         | float float | relative coordinates of eye 1 in right image                 |
| right_2         | float float | relative coordinates of eye 2 in right image                 |
| right_3         | float float | relative coordinates of mouth in right image                 |
| right_4         | float float | relative coordinates of nose in right image                  |


## Folder structure

* The dataset was split into multiple folders (one for each volunteer)
* Each folder is further subdivided into 2 folder (registered and unregistered images) and 1 file (data.csv) containing the portion of the dataset corresponding to the volunteer


## Images name format

{sufix}__{timestamp}.png

* **sufix:** indicates the type of image(uil = unregistered images left, uir = unregistered images right, ril = registered images left, rir = registered images right)
* **timestamp:** timestamp with format "%Y-%m-%d__%H:%M:%S.%f" that indicates when was the height measurement taken


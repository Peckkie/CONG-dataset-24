## Additional explanation
There are 2 important CSV files

<details open>
<summary>"CONG-CODE-YT.csv"</summary>
  
[**"CONG-CODE-YT.csv"**](https://github.com/Peckkie/CONG-dataset-24/blob/main/CONG-CODE-YT.csv) contains data related to the codes that will specify the location and time range of videos on YouTube.
It will have 10 columns: video_name, task_name, start, stop, idx_people, class, idx_class, class_time_start, class_time_stop, and video_split.

**Metadata**

|   Columns name   |                                                        Description                                                        | Candidate key |
|:----------------:|:-------------------------------------------------------------------------------------------------------------------------:|:-------------:|
| video_name       | The name of the video that can specify the location of the video on YouTube.                                              |               |
| task_name        | The name of the sub-video that has been segmented into clips based on time intervals.                                     |       ✔️       |
| start            | The time period when the event of interest begins.                                                                        |               |
| stop             | The time period when the event of interest ends.                                                                          |               |
| idx_people       | The index of the individuals in the video clip to track them individually.                                                |       ✔️       |
| class            | The type of person that has been specified, which can be one of three categories: Gun,  ConcealedGun, and UnconcealedGun. |               |
| idx_class        | The index of the class.                                                                                                   |               |
| class_time_start | The start time when the person appears in the video footage.                                                              |               |
| class_time_stop  | The end time when the person appears in the video footage.                                                                |               |
| video_split      | The subset of data that has been specified for Train/Test.                                                                |               |

</details>

<details open>
<summary>"vdo-box-annotated.csv"</summary>

[**"vdo-box-annotated.csv"**](https://github.com/Peckkie/CONG-dataset-24/blob/main/vdo-box-annotated.csv)
contains annotation data related to the Person Boxes of each individual in each video.

</details>


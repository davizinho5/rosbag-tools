# ROSBag Tools

Use `python3 <script> --help` to print documentation for each of the
following scripts.

| Script                | Description                             |
|:----------------------|:----------------------------------------|
| `bag2csv.py`          | convert all the topics in a bag file into a csv
| `bag2csv_extra.py`    | convert topics in a bag file into a csv
| `bag2images.py`       | convert the given image topic to png images into the given folder
| `bag2video.py`        | convert a ROS bag with image topic to a video file.
| `clip.py`             | extract clips from a bag file using a sentinel topic and range of message indexes
| `decompress.py`       | decompress compressed image data to raw image data
| `dump.py`             | dump messages to the terminal and optionally to disk
| `extract_depth.py`    | extract depth measures to NumPy compressed tensors
| `merge.py`            | merge bag files and filter for certain topics
| `play_depth.py`       | play image and depth data to pyglet windows
| `play_images.py`      | play raw image data to pyglet windows
| `play_super_pixel.py` | play raw image data through a super pixel segmentation algorithm to a pyglet window
| `semantic_segment.py` | produce samples from a semantic segmentation model and an image topic
| `shift.py`            | shift a topic in by an offset in seconds
| `video_to_bag.py`     | convert a video file to a ROS bag


## Usage

    $ python bag2csv.py --bags [rosbag1] ... [rosbagN] --topics [topic1] ... [topicN]
    
    
## Arguments Details
  ```
  -h, --help            show this help message and exit
  -b [BAGS [BAGS ...]], --bags [BAGS [BAGS ...]]
                        rosbag filepaths
  -t [TOPICS [TOPICS ...]], --topics [TOPICS [TOPICS ...]]
                        topics name you want to save ( don't forget slash!!)

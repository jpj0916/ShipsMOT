ShipsMOT
ShipsMOT includes both intraclass and interclass variations of ships during sailing, covering categories, lighting conditions, and backgrounds. It addresses real-world challenges such as occlusions and object similarities. The dataset contains 15 ship categories, over 50,000 frames, and 230,000 bounding boxes, providing comprehensive resources for training detection and tracking models.

The dataset is available at www.baiduyun.com

Details
ShipsMOT is composed of videos sourced from live maritime surveillance systems and the Internet to enhance trajectory diversity. All videos feature resolutions of 1920×1080 or 1280×720, with durations ranging from tens of seconds to minutes. Selected based on public availability, high ship trajectory density, and diverse backgrounds, the dataset ensures comprehensive coverage of real-world maritime scenarios.

ShipsMOT is annotated in MOT format, a specialized standard for multi-object tracking that precisely captures the motion trajectories and states of multiple objects within video sequences. Each frame's data comprises nine distinct fields, enabling detailed tracking of ships' movements and interactions across the dataset.

Position	Name	Description
1	Frame	The number of frames
2	Id	The number of tracks
3	Bb_left	The coordinates of the upper left corner of the bounding box and the length and width of the object
4	Bb_top	The coordinates of the upper left corner of the bounding box and the length and width of the object
5	Bb_width	The coordinates of the upper left corner of the bounding box and the length and width of the object
6	Bb_height	The coordinates of the upper left corner of the bounding box and the length and width of the object
7	Conf	The confidence level
8	X	The content used in MOT3D is always -1 in 2D detection
9	Y	The content used in MOT3D is always -1 in 2D detection
Dataset variety
Category Variation ShipsMOT includes 15 categories common in real-world ship sailing scenarios, helping models refine the understanding of general ship features and attributes for more accurate detection and tracking.



Background Variation It covers six distinct water environments (e.g., city, coast, harbor) to capture ships’ sailing status across real-world water scenarios, enhancing the model’s generalization and practical applicability.



Illumination Variation Object images under diverse lighting conditions—sunny days, cloudy days, sunrise, sunset, and night—are included to ensure robust performance in various lighting scenarios for ship detection and tracking.



Viewpoint Variation Integrates multiple viewpoints (aerial, side, front views) and observations from different positions/altitudes, offering rich viewpoint diversity for model training.



Scale Variation Contains ships of various scales, from large passenger ships/oil carriers to small crafts (canoes, kayaks), and includes scale differences of the same ship type due to distance variations.



Occlusion Scenarios Incorporates scenarios where ships are partially/fully occluded by other ships, buildings, or natural scenery, evaluating tracking methods’ performance in handling occlusions for detection and multi-object tracking.



Object Similarity Includes numerous videos of ships with similar appearances during real-world sailing/berthing, improving the Re-ID performance of tracking models.



Deformation of the Same Object Contains videos of the same object’s deformation (scale and viewpoint changes) caused by distance and viewpoint variations in real sailing environments.



Dataset statistics
Dataset split ShipsMOT contains 121 videos, with 81 videos designated for training and 40 for testing. Both the training and testing annotations are publicly available for research purposes.

Split	Category	Sequences	Avg. len. (s)	Tracklets	Bounding boxes
train	15	81	16.5	457	185128
test	15	40	14.4	151	52871
Total	15	121	15.45	608	237999
Data classification The diverse category distribution and substantial number of training samples facilitate comprehensive model learning of ship features, thereby improving detection and multi-object tracking precision and generalization capabilities.

Category	Bounding boxes
Passenger ship	58848
Container ship	13917
Sailing ship	20174
Speed boat	21589
Barge	1734
Fishing boat	26824
Ferry boat	15490
General cargo ship	15506
Oil carrier	3862
Canoe	22610
Tug	8229
Warship	426
Kayak	1009
Ore carrier	8591
Bulk cargo carrier	19190
image-20250321105807560

Scale	Pixel area	Number of Objects
Small	<=32×32	32426
Medium	>32×32，<=96×96	125469
Large	>96×96	80104

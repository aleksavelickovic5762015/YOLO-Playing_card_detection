# YOLO-detection

Видео на коме је извршена детекција карата:
https://drive.google.com/file/d/1-Jd3jtQmfzYIymziRFvmzKLNjx7yzGqo/view?usp=drivesdk

Тежински коефицијенти истрениране мреже:
https://drive.google.com/file/d/1-2HHIq1DWr3cKZ7LTFsWU1TEIZnFhq_q/view?usp=sharing

Сваку од 52 карте шпила сам снимио под различитим осветљењем, пример:
https://drive.google.com/file/d/102PA6_wRgA8eTqtfgw9l7Mrq5TbDXe44/view?usp=drivesdk

Из сваког видеа тј. за сваку карту се добије око 100 слика.
Дефинисао сам позицију правоугоника, тако да одговара мом шпилу и прецизно окружи знак и број карте.
Онда се позива функција која унутар тако дефинисаног правоугаоника, црта неправилан полигон око знака и броја.
Скуп за тренирање се генерише подвлачењем једне од много позадина испод карата.
Пола скупа је генерисано насумичним транслирањем, ротацијом и увећавањем две карте; у другој половини су карте такође насумично позициониране, али сад једна до друге као када се држе у руци.
На крају се позива пајтон функција која позиције генерисаних карата из XML датотеке преводи у формат који одговара YOLO и уписује у txt датотеку.
Тренинг скуп садржи 50000 слика, валидациони 10000.
Гитхаб репозиторијум за генрисање тренинг података:
https://github.com/geaxgx/playing-card-detection

Тренирање је изршено коришћењем Darknet фрејмворка:
https://github.com/AlexeyAB/darknet

Користио сам виртуелну машину на GoogleColaboratory за тренирање, линк на свеску:
https://colab.research.google.com/drive/1_GdoqCJWXsChrOiY8sZMr_zbr_fH-0Fg?usp=sharing

Линк на два видеа са YouTube...

Поступак припреме слика и промене параметара током тренирања:
https://youtu.be/pnntrewH0xg

Коришћење Darknet у GoogleColaboratory:
https://youtu.be/mmj3nxGT2YQ


=====================================================================

(ENG)

Card detection video result:
https://drive.google.com/file/d/1-Jd3jtQmfzYIymziRFvmzKLNjx7yzGqo/view?usp=drivesdk

Weights of trained network:
https://drive.google.com/file/d/1-2HHIq1DWr3cKZ7LTFsWU1TEIZnFhq_q/view?usp=sharing

Every card from 52 card deck was filmed in different lighting conditions, example:
https://drive.google.com/file/d/102PA6_wRgA8eTqtfgw9l7Mrq5TbDXe44/view?usp=drivesdk

From every video, i.e. for every card there are 100 images.
Rectangle that surrounds card value is defined to fit card deck that is used.
Then the function that creates a polygon around the card value (inside defined rectangle) is called.
Training set is created by random positioning of a card on a random backround image.
Half of the training set is created by translation, rotation and zooming of two cards: and the other half contains images of three cards, one next to the other, randomly positioned.
Python function transforms card position data in XML file to the YOLO format, and writes it to txt file.
Training dataset contains 50000 images, validation dataset 10000.
Github repository for creatnig dataset:
https://github.com/geaxgx/playing-card-detection

Training of the dataset was done using Darknet framework:
https://github.com/AlexeyAB/darknet

I used GoogleColaboratory for running the framework, jupyter notebook:
https://colab.research.google.com/drive/1_GdoqCJWXsChrOiY8sZMr_zbr_fH-0Fg?usp=sharing

YouTube videos:

Creating dataset, changing training parameters:
https://youtu.be/pnntrewH0xg

Using Darknet in GoogleColaboratory:
https://youtu.be/mmj3nxGT2YQ

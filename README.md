# Diplomski-rad---YOLO-detekcija

Видео на коме је извршена детекција карата:
https://drive.google.com/file/d/1-Jd3jtQmfzYIymziRFvmzKLNjx7yzGqo/view?usp=drivesdk

Тежински коефицијенти истрениране мреже:
https://drive.google.com/file/d/1-2HHIq1DWr3cKZ7LTFsWU1TEIZnFhq_q/view?usp=sharing

Сваку од 52 карте шпила сам снимио под различитим осветљењем, пример:
https://drive.google.com/file/d/102PA6_wRgA8eTqtfgw9l7Mrq5TbDXe44/view?usp=drivesdk

Из сваког видеа тј. за сваку карту се добије око 100 слика.
Дефинисао сам позицију правоугоника, тако да одговара мом шпилу и прецизно окружи знак и број карте.
Онда се позива функција, која унутар тако дефинисаног правоугаоника, црта неправилан полигон око знака и броја.
Скуп за тренирање се генерише подвлачењем једне од много позадина испод карата.
Пола скупа је генерисано насумичним транслирањем, ротацијом и увећавањем две карте; у другој половини су карте такође насумично позициониране, али сад једна до друге као када се држе у руци.
На крају се позива пајтон функција која позиције генерисаних карата из XML датотеке преводи у формат који одговара YOLO и уписује у txt датотеку.
Тренинг скуп садржи 50000 слика, валидациони 10000.
Гитхаб репозиторија за генрисање тренинг података:
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

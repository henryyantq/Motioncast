# Motioncast
日前，我们构思了一种移动端的动作识别方案，可以将移动端运动传感器采集得到的时序数据映射为标签化的二维图像，并期望通过训练图像分类器的方法得到一个可以进行动作识别的神经网络模型。这个项目的意义在于，我们希望这能助推更有潜力的体感交互系统。为此，我们在安卓端开发出了Motioncast，采用构思的运动学数据采集和映射方式让我们能够记录任何一系列动作的传感器数据并输出（映射）为一个九通道的彩色图像。  为了初步试验这种数据采集和映射的方案是否有效，我进行了一个简单、粗糙的样本采集+模型训练和测试。  使用Motioncast分别采集了14和17张在空中挥动手势比划数字“2”和“3”的九通道传感器数据映射彩图，并作为训练样本丢入神经网络训练出了一个最简单的图像分类器。接着，我将15张新采集得到的“2”或“3”彩图作为测试样本丢入训练好的模型，得到的测试结果如图所示，正确率为66.6%，即15张测试样本中有5张被误识别为了另一个数字。  超过了50%的正确率让我们对这种动作识别方案增添了一些信心，但66.6%的正确率对于一个神经网络模型来说并不算成功。目前，由于知识水平有限，我们只能暂时忽略本身这种样本生成算法——即Motioncast对传感器数据的采集和映射方法存在的问题，而更关注其它的可控因素，包括训练样本的数量、训练方式、神经网络模型参数等是否存在改进空间。目前，最大的难题可能在于无法获得大量的训练和测试样本，这可能会使得我们一段时间内无法真正得到足够优秀（至少足够充分）的测试结果来验证Motioncast这种运动传感器数据映射算法的有效性。

本人的联系方式：1580955042@qq.com

![image](https://user-images.githubusercontent.com/20149275/117971091-05c39900-b35c-11eb-8f04-69ad9465c26b.png)

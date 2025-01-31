.. _cn_api_paddle_nn_functional_thresholded_relu:

thresholded_relu
-------------------------------

.. py:function:: paddle.nn.functional.thresholded_relu(x, threshold=1.0, value=0.0, name=None)

thresholded relu 激活层。计算公式如下：

.. math::

    thresholded\_relu(x) =
        \left\{
            \begin{array}{rl}
            x,& \text{if } \ x > threshold \\
            value,& \text{otherwise}
            \end{array}
        \right.

其中，:math:`x` 为输入的 Tensor。


参数
::::::::::
    - **x** (Tensor) - 输入的 ``Tensor``，数据类型为：float32、float64。
    - **threshold** (float，可选) - thresholded_relu 激活计算公式中的 threshold 值。默认值为 1.0。
    - **value** (float，可选) - 当 ``x`` 小于 ``threshold`` 时的替换值。默认值为 0.0。
    - **name** (str，可选) - 具体用法请参见 :ref:`api_guide_Name`，一般无需设置，默认值为 None。

返回
::::::::::
    ``Tensor``，数据类型和形状同 ``x`` 一致。

代码示例
::::::::::

COPY-FROM: paddle.nn.functional.thresholded_relu

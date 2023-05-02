# Italian to English Translation

## Translation Results
+-------------------+------------+---------------------------------+--------------------------------+
|       Model       | BLUE score |              Actual             |           Predicted            |
+-------------------+------------+---------------------------------+--------------------------------+
|  Encoder Decoder  |   0.3911   | Why didn't Tom come back? <end> |    why didn't tom come back    |
|   Attention dot   |   0.4888   | Why didn't Tom come back? <end> |    why did tom is tom <end>    |
| Attention general |   0.4166   | Why didn't Tom come back? <end> |       i don't you <end>        |
|  Attention concat |   0.5996   | Why didn't Tom come back? <end> | why didn't tom come back <end> |
+-------------------+------------+---------------------------------+--------------------------------+

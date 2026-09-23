<img width="887" height="622" alt="屏幕截图 2026-09-23 222021" src="https://github.com/user-attachments/assets/eebb856c-7b37-497b-a289-eba852b49f4a" />
<img width="603" height="441" alt="屏幕截图 2026-09-23 221737" src="https://github.com/user-attachments/assets/3155a5ba-24cc-4ed2-a3d4-ef5f7d1e7336" />



说明：芯片型号为STM32F407VGTx，将PE5配置为GPIO推挽输出，用来控制LED；PH0、PH1用作外部高速晶振HSE的输入输出引脚，为系统提供外部时钟源。
说明：系统时钟由HSE（8MHz外部晶振）作为PLL输入源，经过PLL倍频后，系统主时钟SYSCLK配置为168MHz。AHB预分频系数为1，HCLK=168MHz；APB1预分频系数为4，PCLK1=42MHz；APB2预分频系数为2，PCLK2=84MHz

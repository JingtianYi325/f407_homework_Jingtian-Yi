<img width="860" height="613" alt="屏幕截图 2026-09-23 222930" src="https://github.com/user-attachments/assets/093bbd5e-45f0-4216-a3ed-a6e9580e4f60" />
<img width="545" height="458" alt="屏幕截图 2026-09-23 222859" src="https://github.com/user-attachments/assets/d0de8d36-2d8c-4847-a5a2-28a879bd2e79" />


引脚配置:
PE5、PE6：设置为GPIO_Output（推挽输出），用于驱动LED;PA0;  设置为GPIO_Input，用作按键输入;  PH0、PH1：分配为RCC_OSC_IN、RCC_OSC_OUT，接入8MHz外部高速晶振HSE。
时钟树配置:
以HSE 8MHz作为PLL时钟输入源；HSE先4分频，再168倍频，再2分频，得到PLLCLK=168MHz。系统时钟SYSCLK选择PLLCLK，主频168MHz。
AHB预分频系数：1，HCLK=168MHz
APB1预分频系数：4，PCLK1=42MHz，APB1定时器时钟为84MHz
APB2预分频系数：2，PCLK2=84MHz，APB2定时器时钟为168MHz

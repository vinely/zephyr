#
# Copyright (c) 2018, NXP
#
# SPDX-License-Identifier: Apache-2.0
#

zephyr_include_directories(.)

zephyr_sources_ifdef(CONFIG_ADC_MCUX_ADC16    fsl_adc16.c)
zephyr_sources_ifdef(CONFIG_ETH_MCUX          fsl_enet.c)
zephyr_sources_ifdef(CONFIG_I2C_MCUX          fsl_i2c.c)
zephyr_sources_ifdef(CONFIG_PWM_MCUX_FTM      fsl_ftm.c)
zephyr_sources_ifdef(CONFIG_ENTROPY_MCUX_RNGA fsl_rnga.c)
zephyr_sources_ifdef(CONFIG_ENTROPY_MCUX_TRNG fsl_trng.c)
zephyr_sources_ifdef(CONFIG_SOC_FLASH_MCUX    fsl_flash.c)
zephyr_sources_ifdef(CONFIG_SPI_MCUX_DSPI     fsl_dspi.c)
zephyr_sources_ifdef(CONFIG_UART_MCUX         fsl_uart.c)
zephyr_sources_ifdef(CONFIG_UART_MCUX_LPSCI   fsl_lpsci.c)
zephyr_sources_ifdef(CONFIG_UART_MCUX_LPUART  fsl_lpuart.c)
zephyr_sources_ifdef(CONFIG_RTC_MCUX          fsl_rtc.c)
zephyr_sources_ifdef(CONFIG_WDT_MCUX_WDOG     fsl_wdog.c)

#
# Copyright (c) 2020 Nordic Semiconductor
#
# SPDX-License-Identifier: LicenseRef-BSD-5-Clause-Nordic
#
cmake_minimum_required(VERSION 3.13.1)

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(entropy_nrf53_cpuapp)

# NORDIC SDK APP START
target_sources(app PRIVATE
  src/main.c
  src/entropy_ser.c
)
# NORDIC SDK APP END

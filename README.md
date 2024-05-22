# Boost Converter Design and Testing for Voltage Step-Up

## Project Overview

This project involves the design and testing of a Boost Converter that steps up voltage from 15V to 25V and 30V, meeting a 20W power output target. Boost converters, also known as step-up converters, are DC-to-DC power converters widely used in applications such as battery-powered devices, LED lighting, and renewable energy systems.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Designed Parameters](#designed-parameters)
- [Working Principle](#working-principle)
- [Formulas](#formulas)
- [Circuit Diagram](#circuit-diagram)
  

## Introduction

Boost converters are essential components in power electronics for increasing the voltage level of a DC source. This project aims to design and test a boost converter that can convert a 15V DC input to two output voltages, 25V and 30V, with a maximum output power of 20W.

## Features

- **Voltage Step-Up**: Converts 15V DC input to 25V and 30V DC outputs.
- **Power Output**: Achieves a maximum output power of 20W.
- **High Efficiency**: Optimized component values for continuous current mode.
- **Reliable Components**: Uses MOSFET IRF540N and diode IN5408.
- **Optimized Design**: Ensures minimal voltage ripple with appropriate inductor and capacitor values.

## Designed Parameters

| Parameter                | Value      |
|--------------------------|------------|
| Input Voltage            | 15V DC     |
| Output Voltage (25V)     | 25V DC     |
| Output Voltage (30V)     | 30V DC     |
| Maximum Output Power     | 20W        |
| Switching Frequency      | 20 kHz     |
| Inductor Value           | 18mH       |
| Output Capacitor Value   | 100µF      |
| Switching Element        | MOSFET IRF540N |
| Diode                    | IN5408     |

## Working Principle

A boost converter operates by storing energy in an inductor during the on-time of a switching element (typically a MOSFET) and releasing that energy to the output during the off-time. This process effectively increases the voltage level at the output.

## Formulas

- **Output Voltage**: \( V_o = \frac{V_s}{1 - D} \)
- **Minimum Inductance for Continuous Current**: \( L_{min} = \frac{D (1 - D)^2}{2f} \)
- **Inductor Current**: \( I_L = \frac{V_s}{R (1 - D)^2} \)
- **Minimum Capacitance to Limit V\(_0\) Ripple to 1%**: \( C_{min} = \frac{D}{R (\Delta V_0 / V_0) f} \)

## Circuit Diagram
![image](https://github.com/Vishnu45t86/Boost-converter/assets/109750872/0d2074bf-9605-4f68-b621-87b1c96e843f)



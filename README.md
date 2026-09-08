# EXP-5: Comparing Prompting Techniques Through Engineering Problem-Solving Scenarios
# Reg no: 212224243001
## Experiment Title

**Comparing Prompting Techniques Through Engineering Problem-Solving Scenarios**

---

## Aim

To compare different prompting techniques and evaluate their effectiveness in solving a real-world engineering problem by using the **Smart Energy Meter using IoT** project as the engineering scenario.

The experiment focuses on understanding how different prompting techniques affect the **quality, accuracy, completeness, clarity, feasibility, and usefulness** of AI-generated solutions.

---

## Engineering Project Selected

### Project Title

**IoT-Based Smart Energy Meter**

### Problem Statement

Traditional electricity meters mainly provide energy consumption information locally and may not provide real-time monitoring or remote access.

The proposed IoT-based Smart Energy Meter measures electrical parameters such as voltage, current, power, and energy consumption. The measured data can be displayed locally and monitored remotely using an IoT platform.

The system uses an **ESP32 microcontroller**, current and voltage sensing, an **I2C LCD display**, and an IoT platform for monitoring.

---

# 1. Selected Engineering Scenario

### Scenario

Design an **IoT-based Smart Energy Meter** capable of:

- Measuring voltage
- Measuring current
- Calculating power
- Calculating energy consumption
- Displaying readings on an LCD
- Sending data to an IoT platform
- Allowing remote monitoring
- Providing a simple and low-cost implementation
- Providing reliable and readable measurements

### Main Components

- ESP32 Microcontroller
- Voltage Sensor
- Current Sensor
- I2C LCD Display
- Wi-Fi
- IoT Platform
- Power Supply
- Electrical Load

---

# 2. Prompt Chain

The following prompt chain was used to solve the selected engineering problem.

```text
Engineering Problem
        ↓
Requirement Analysis
        ↓
Architecture Design
        ↓
Flowchart
        ↓
Implementation / Python Code
        ↓
Testing
        ↓
Documentation
        ↓
Final Engineering Solution
```
# 3. Base Prompt
Base Prompt
```
Design an IoT-based Smart Energy Meter using ESP32. 
The system should measure voltage, current, power and energy consumption.
Display the readings on an I2C LCD and send the data to an IoT platform
for remote monitoring. Explain the components, working principle,
architecture, flowchart, implementation and testing procedure.
Purpose
```

The base prompt provides a general description of the project without using any advanced prompting technique.

# 4. Prompting Technique 1 – Zero-Shot / Straightforward Prompting
```
Design an IoT-based Smart Energy Meter using ESP32.
The system should measure voltage, current, power and energy consumption.
Display the readings on an I2C LCD and send the data to an IoT platform
for remote monitoring. Explain the components and working principle.
```
AI-Generated Output

The AI suggested an IoT-based energy monitoring system using an ESP32.

The basic system contains:

ESP32 microcontroller
Voltage sensor
Current sensor
I2C LCD
Wi-Fi connection
IoT cloud platform

The ESP32 collects voltage and current measurements from the sensors.

# 5. Prompting Technique 2 – Role-Based Prompting
Prompt
Act as an experienced Embedded Systems and IoT Engineer.

Design an IoT-based Smart Energy Meter using ESP32, voltage sensing,
current sensing, I2C LCD and Wi-Fi.

Provide:

1. Component selection
2. Hardware architecture
3. Software architecture
4. Measurement equations
5. Data flow
6. IoT communication method
7. Testing procedure
8. Possible errors and troubleshooting methods

Explain the solution in a way that a third-year engineering student
can understand and implement.
AI-Generated Output

The AI approached the problem from an embedded systems engineering perspective.

Hardware
ESP32 acts as the main controller.
Voltage sensing circuit measures the supply voltage.
Current sensor measures load current.
I2C LCD provides local display.
Wi-Fi provides communication with the IoT platform.
Measurement

The basic power calculation is:

P = V × I

Energy can be calculated as:

Energy = Power × Time

For practical implementation, sensor calibration is required before using the measured values.

Software

The ESP32 program should:

Initialize sensors.
Initialize LCD.
Connect to Wi-Fi.
Read voltage.
Read current.
Calculate power.
Calculate energy.
Display readings.
Send readings to the IoT platform.
Repeat continuously.
Observation

Role-based prompting produced a more structured engineering response with better consideration of implementation and testing.

# 6. Prompting Technique 3 – Step-by-Step Prompting
Prompt
Solve the following engineering problem step by step.

Problem:
Develop an IoT-based Smart Energy Meter using ESP32.

Step 1: Identify the functional requirements.
Step 2: Identify hardware components.
Step 3: Design the system architecture.
Step 4: Explain voltage and current measurement.
Step 5: Explain power and energy calculation.
Step 6: Explain LCD interfacing.
Step 7: Explain Wi-Fi and IoT communication.
Step 8: Create the system flow.
Step 9: Provide implementation logic.
Step 10: Explain testing and validation.

Clearly explain each step and mention important assumptions.
AI-Generated Output
Step 1 – Functional Requirements

The system should:

Measure voltage.
Measure current.
Calculate power.
Calculate energy.
Display readings.
Send readings through Wi-Fi.
Allow remote monitoring.
Step 2 – Hardware Components
ESP32
Voltage Sensor
Current Sensor
I2C LCD
Power Supply
Load
Wi-Fi
Step 3 – Architecture
Electrical Load
      ↓
Voltage / Current Sensors
      ↓
ESP32
   ↙     ↘
LCD     Wi-Fi
          ↓
    IoT Platform
          ↓
   Remote Monitoring
Step 4 – Measurement

The sensors provide electrical measurements to the ESP32.

The ESP32 processes the sensor readings and converts them into useful engineering parameters.

Step 5 – Power Calculation
P = V × I

where:

P = Power in watts
V = Voltage in volts
I = Current in amperes
Step 6 – Energy Calculation

Energy is obtained from power over time.

Energy = Power × Time

For electrical energy measurement, appropriate time units and conversion factors must be used.

Step 7 – LCD

The I2C LCD is connected to the ESP32 using the I2C communication interface.

It displays parameters such as:

Voltage: XX V
Current: XX A
Power: XX W
Energy: XX kWh
Step 8 – IoT Communication

The ESP32 connects to a Wi-Fi network and sends measured data to the selected IoT platform.

Step 9 – Implementation Logic
Start
  ↓
Initialize ESP32
  ↓
Initialize Sensors
  ↓
Initialize LCD
  ↓
Connect Wi-Fi
  ↓
Read Voltage
  ↓
Read Current
  ↓
Calculate Power
  ↓
Calculate Energy
  ↓
Display Data on LCD
  ↓
Send Data to IoT Platform
  ↓
Repeat
Step 10 – Testing

The system can be tested using different electrical loads and comparing measured values with reference measurements.

Observation

Step-by-step prompting provided a more complete and organized solution because the problem was divided into smaller engineering tasks.

# 7. Prompting Technique 4 – Few-Shot / Example-Based Prompting
Prompt
You are designing an IoT-based Smart Energy Meter.

Example format:

Example 1:
Input: Measure voltage and current.
Output:
- Read voltage sensor.
- Read current sensor.
- Convert sensor values.
- Apply calibration.
- Display the values.

Example 2:
Input: Calculate electrical power.
Output:
Power = Voltage × Current

Now solve the complete Smart Energy Meter problem using the same
structured format.

Include:
1. Requirements
2. Components
3. Architecture
4. Sensor measurement
5. Power calculation
6. Energy calculation
7. LCD display
8. IoT communication
9. Testing
10. Troubleshooting
AI-Generated Output

The AI followed the example structure and produced a structured solution.

Requirement

The system should continuously monitor electrical parameters and make the information available locally and remotely.

Component Selection
Component	Purpose
ESP32	Main controller
Voltage Sensor	Voltage measurement
Current Sensor	Current measurement
I2C LCD	Local display
Wi-Fi	Internet communication
IoT Platform	Remote monitoring
Processing
Sensor Reading
      ↓
Calibration
      ↓
ESP32 Processing
      ↓
Voltage + Current
      ↓
Power Calculation
      ↓
Energy Calculation
IoT
ESP32 → Wi-Fi → IoT Platform → Dashboard
Testing

Test the system using different load conditions and compare the measured values against reference values.

Observation

Few-shot prompting improved the consistency and structure of the generated response because examples were provided before asking for the final solution.

# 8. Prompting Technique 5 – Constraint-Based Prompting
Prompt
Design an IoT-based Smart Energy Meter using ESP32.

Follow these constraints:

1. Use ESP32 as the main controller.
2. Use an I2C LCD for local display.
3. Use Wi-Fi for communication.
4. The solution must be low-cost.
5. The explanation must be suitable for a third-year ECE student.
6. Clearly separate hardware and software.
7. Include power and energy calculations.
8. Include testing and validation.
9. Mention sensor calibration.
10. Mention electrical safety considerations.
11. Avoid unnecessary components.
12. Provide a practical implementation approach.
AI-Generated Output

The constraint-based prompt generated a more focused solution.

Hardware
Voltage Sensor
       ↓
Current Sensor → ESP32 → I2C LCD
                   ↓
                 Wi-Fi
                   ↓
             IoT Platform
Important Constraints

The design should use minimum hardware while maintaining sufficient measurement accuracy.

Sensor calibration should be performed before deployment.

Electrical isolation and proper safety precautions should be considered when working with mains electricity.

Testing

The system should be tested under different load conditions.

Measured values should be compared with reference values.

Observation

Constraint-based prompting reduced irrelevant information and produced a solution that was more closely aligned with the actual project requirements.

# 9. Comparison of Prompting Techniques
Criteria	Base Prompt	Zero-Shot	Role-Based	Step-by-Step	Few-Shot	Constraint-Based
Relevance	3/5	3/5	5/5	5/5	4/5	5/5
Accuracy	3/5	3/5	4/5	4/5	4/5	5/5
Completeness	2/5	3/5	4/5	5/5	4/5	5/5
Clarity	3/5	3/5	5/5	5/5	4/5	5/5
Feasibility	3/5	3/5	4/5	4/5	4/5	5/5
Usefulness	3/5	3/5	5/5	5/5	4/5	5/5
Engineering Depth	2/5	3/5	5/5	5/5	4/5	5/5
Overall Observation

The results show that prompts containing clear roles, step-by-step instructions, examples, and constraints generally produced more useful engineering responses than simple prompts.

# 10. Analysis and Observations

The experiment demonstrates that prompt structure has a significant effect on AI-generated engineering solutions.

Base / Naive Prompt

The base prompt generated a general solution.

However, it did not provide enough constraints or implementation details.

Zero-Shot Prompt

The zero-shot prompt was useful for obtaining a quick initial solution.

It was suitable for understanding the general concept but lacked engineering depth.

Role-Based Prompt

Role-based prompting improved the response by asking the AI to behave like an experienced Embedded Systems and IoT Engineer.

This resulted in better technical organization and practical suggestions.

Step-by-Step Prompt

Step-by-step prompting produced one of the most complete responses.

Breaking the engineering problem into smaller tasks helped generate a systematic solution.

Few-Shot Prompt

Few-shot prompting improved consistency by providing examples of the expected response format.

Constraint-Based Prompt

Constraint-based prompting produced a focused and practical solution because the AI was given specific project limitations and requirements.

# 11. Why Prompt Clarity Matters

A vague prompt can produce a generic answer.

For example:

Design a smart energy meter.

This does not specify:

Controller
Sensors
Communication method
Display
Calculations
Testing requirements
Cost constraints

A clearer prompt provides better guidance:

Design a low-cost IoT-based Smart Energy Meter using ESP32,
voltage and current sensors, I2C LCD and Wi-Fi.
Explain the architecture, calculations, implementation,
testing and safety considerations.

The second prompt provides more context and therefore generates a more useful engineering response.

# 12. Final Selected Prompting Technique
Selected Technique

Constraint-Based + Step-by-Step Prompting

The combination of constraint-based and step-by-step prompting was selected as the most effective technique for this engineering problem.

Reason for Selection

This technique:

Provides clear project requirements.
Reduces irrelevant information.
Produces structured answers.
Covers hardware and software.
Includes testing and validation.
Considers practical constraints.
Is easier for engineering students to implement.
Improves the depth and usefulness of the AI response.

# 13. Refined / Final Prompt
Act as an experienced Embedded Systems and IoT Engineer.

Design a practical, low-cost IoT-based Smart Energy Meter using ESP32.

Project requirements:

1. Use ESP32 as the main microcontroller.
2. Measure voltage and current using appropriate sensors.
3. Calculate electrical power using measured voltage and current.
4. Calculate accumulated energy consumption.
5. Display voltage, current, power and energy on an I2C LCD.
6. Use Wi-Fi to send measurements to an IoT monitoring platform.
7. Provide a clear hardware and software architecture.
8. Provide a complete system flowchart.
9. Explain the working principle step by step.
10. Provide implementation logic or suitable code structure.
11. Explain sensor calibration and measurement errors.
12. Provide a testing procedure using different load conditions.
13. Explain how measured values can be validated against a reference meter.
14. Mention electrical safety and isolation requirements.
15. Keep the solution suitable for a third-year ECE engineering project.
16. Avoid unnecessary components and features.

Present the answer in the following order:

A. Problem Statement
B. Requirements
C. Components
D. Hardware Architecture
E. Software Architecture
F. Working Principle
G. Mathematical Calculations
H. Flowchart
I. Implementation
J. Testing
K. Troubleshooting
L. Engineering Validation
M. Expected Result
N. Conclusion

# 14. Engineering Validation

The AI-generated design should not be accepted directly without practical verification.

The following parameters can be validated experimentally:

Parameter	AI Calculation	Reference Measurement	Validation
Voltage	ESP32 sensor reading	Reference meter	Compare
Current	Current sensor reading	Reference meter	Compare
Power	V × I	Reference power value	Compare
Energy	Accumulated power over time	Energy meter	Compare
IoT Data	ESP32 transmitted value	Dashboard value	Verify
LCD Data	ESP32 processed value	LCD display	Verify
Validation Procedure
Connect the selected load safely.
Measure voltage using a reference instrument.
Measure current using a reference instrument.
Record the ESP32 sensor readings.
Compare sensor values with reference values.
Calculate percentage error.
Check LCD readings.
Check IoT dashboard readings.
Repeat the experiment with different load conditions.
Analyze the consistency of the measurements.
Percentage Error
Percentage Error =
|Measured Value - Reference Value|
---------------------------------- × 100
        Reference Value
		
# 15. Testing

The following tests can be performed.

Test 1 – Power ON Test

Check whether the ESP32, LCD and sensors initialize correctly.

Test 2 – Sensor Test

Verify whether voltage and current sensors provide reasonable readings.

Test 3 – LCD Test

Verify whether the LCD displays:

Voltage
Current
Power
Energy

correctly.

Test 4 – Wi-Fi Test

Verify that the ESP32 successfully connects to the configured Wi-Fi network.

Test 5 – IoT Data Test

Check whether sensor data reaches the IoT dashboard correctly.

Test 6 – Load Variation Test

Test the system with different load conditions and observe changes in:

Voltage
Current
Power
Energy
Test 7 – Long Duration Test

Run the system continuously and verify whether the readings remain stable.

# 16. Expected Result

The proposed IoT-based Smart Energy Meter should:

Measure electrical parameters.
Calculate power and energy consumption.
Display readings on an I2C LCD.
Transmit data using Wi-Fi.
Provide remote monitoring through an IoT platform.
Produce reasonably accurate measurements after calibration.
Demonstrate the practical use of IoT in energy monitoring.

# 17. Prompting Technique Comparison Summary
Prompting Method	Main Advantage	Limitation
Base Prompt	Simple and quick	Less detailed
Zero-Shot	Fast initial solution	Generic response
Role-Based	Better domain perspective	May still need constraints
Step-by-Step	Systematic and complete	Longer prompt
Few-Shot	Consistent output format	Requires useful examples
Constraint-Based	Focused and practical	Requires clearly defined constraints

# 18. Key Findings

The experiment produced the following findings:

Prompt quality directly influences AI output quality.
Simple prompts are useful for initial idea generation.
Role-based prompts improve domain-specific responses.
Step-by-step prompting improves completeness.
Few-shot prompting improves consistency.
Constraint-based prompting improves relevance and feasibility.
Combining multiple prompting techniques can produce better engineering solutions.
AI-generated solutions still require engineering validation.
Sensor calibration and practical testing are essential before using an AI-generated design.
Clear prompts reduce ambiguity and improve the usefulness of AI responses.

# 19. Conclusion

This experiment successfully compared different prompting techniques for solving an engineering problem using an IoT-based Smart Energy Meter as the case study.

The comparison showed that a simple or naive prompt can generate a basic solution, while structured prompting techniques such as Role-Based Prompting, Step-by-Step Prompting, Few-Shot Prompting, and Constraint-Based Prompting can produce more detailed, relevant, and practical engineering solutions.

Among the tested techniques, Constraint-Based + Step-by-Step Prompting was selected as the most suitable approach because it provided clear requirements, systematic reasoning, implementation guidance, testing procedures, and engineering validation.

The experiment demonstrates that effective prompt engineering can improve the usefulness of AI as an engineering problem-solving assistant.


# 20. Result

The experiment was successfully completed. Different prompting techniques were applied to the same engineering problem, and their outputs were compared based on relevance, accuracy, completeness, clarity, feasibility, and usefulness. The Constraint-Based + Step-by-Step prompting approach produced the most structured and practical solution for the selected Smart Energy Meter project.


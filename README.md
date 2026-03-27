# NeuroMap Exporter

NeuroMap Exporter is a cross-platform data processing tool used by research teams to convert and align biomechanical datasets, reducing processing time from **weeks to hours** through automation.

The application enables researchers to transform NeuroMap Explorer data into formats compatible with Visual3D, while handling multi-sensor datasets with differing sampling rates.

Feel free to contact me if there are any issues or if there are any improvements / additional features that could be added

---

## 🧠 Overview

Biomechanical research often involves processing large volumes of data collected from multiple sensors (e.g. IMUs and EMG), each with different sampling frequencies and formats.

NeuroMap Exporter automates this process by:
- Converting proprietary NeuroMap data (.txt format) into analysis-ready formats
- Aligning datasets from multiple sensors
- Upsampling data to ensure consistent sampling rates
- Reducing manual processing effort and human error
  
---

## ✨ Key Features

- ⚡ **Automated Data Conversion**  
  Converts NeuroMap Explorer data into Visual3D-compatible .txt files

- 📊 **Multi-Sensor Data Alignment**  
  Synchronises datasets collected at different sampling rates

- 🖥️ **Cross-Platform Desktop Application**  
  Built using C# and .NET with Avalonia UI

- 🌍 **Real-World Usage**  
  Used by research teams in the UK and internationally

---

## 🛠️ Tech Stack

- **Language:** C#  
- **Framework:** .NET  
- **UI:** Avalonia  
- **Legacy Tooling:** Python (original implementation) [2016]

---

## 🏗️ Architecture

The application is structured around a data processing pipeline:

1. **Input Parsing**  
   - Reads and interprets NeuroMap Explorer data formats  

2. **Data Transformation**  
   - Converts raw data into structured, analysis-ready formats

3. **Alignment & Synchronisation**  
   - Matches datasets from multiple sensors  
   - Handles differing sampling rates  

4. **Upsampling**  
   - Applies interpolation techniques to standardise frequency

5. **Export Layer**  
   - Outputs Visual3D-compatible files (.txt files that can be imported into Visual3D)

---

## 🚀 Getting Started

I have included executables for Windows, Linux and macOS for immediate download and use

### Prerequisites
- .NET SDK installed
- Supported OS: Windows / Linux / macOS

### Running the Application

```bash
git clone https://github.com/jdprichards/neuromap-exporter-dotnet.git
cd neuromap-exporter
dotnet build
dotnet run

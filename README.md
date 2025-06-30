# 17-bit Custom CPU Design
**Course**: Computer Architecture & Design  
**University**: Rajshahi University of Engineering & Technology (RUET)  
**Tools**: Logisim  

## Instruction Set Architecture (17-bit)
### **1. Register Mode (8-bit operands)**
Format: `[2:mode] [1:op] [3:reg1] [3:reg2] [8:unused]`
- **SUB** Example: `00001100100000000`  
  (Mode:00, Op:0, Reg1:110, Reg2:010)  
- **SHL** Example: `00100100100000000`  

### **2. Immediate Mode (5-bit value)**
Format: `[2:mode] [1:op] [3:reg1] [5:value] [6:unused]`
- **SUB** Example: `01001101100000000`  
  (Mode:01, Op:0, Reg1:110, Value:11000)  
- **SHL** Example: `01101101100000000`  

### **3. Branching Mode (4-bit address)**
Format: `[2:mode] [1:op] [4:address] [10:unused]`
- **JGE** Example: `10001100000000000`  
  (Mode:10, Op:0, Address:1100)  

## Project Structure

Skip to content
Navigation Menu
Yuvan2
/
BOOLEAN_FUNCTION_MINIMIZATION

Type / to search
Code
Pull requests
Actions
Projects
Security
Insights
Files
Go to file
t
db
hc_output
incremental_db
output_files
simulation
Boolean_min.qpf
Boolean_min.qsf
Boolean_min.qws
Boolean_min.v
Boolean_min.v.bak
LICENSE
README.md
Waveform2.vwf
c5_pin_model_dump.txt
cio_dump_disallowed_lists.echo
Editing README.md in BOOLEAN_FUNCTION_MINIMIZATION
You’re making changes in a project you don’t have write access to. Submitting a change will write it to a new branch in your fork yogeshwaran72/BOOLEAN_FUNCTION_MINIMIZATION, so you can send a pull request.
BreadcrumbsBOOLEAN_FUNCTION_MINIMIZATION
/
README.md
in
main

Edit

Preview
Indent mode

Spaces
Indent size

2
Line wrap mode

Soft wrap
Editing README.md file contents
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
33
34
35
36
37
38
39
40
41
42
43
44
45
46
47
48
49
50
51
52
53
54
55
56
57
58
59
60
61
62
63
64
65
66
# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

## program
~~~

module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

Developed by:A.yogeshwaran
Register Number:212223040249
~~~

## Logic Symbol and Truth table
![316294107-a6b8101c-bd3c-4b64-bc4a-f4a8962ac13a](https://github.com/04Varsha/BOOLEAN_FUNCTION_MINIMIZATION/assets/149035374/ab520f8d-0d6f-4bb9-96e6-33968a037418)

![316294144-348e89c8-b4d6-4c9e-8783-541ac0829105](https://github.com/04Varsha/BOOLEAN_FUNCTION_MINIMIZATION/assets/149035374/21cb2aef-7529-4ced-a473-68b7a9e53d62)
Use Control + Shift + m to toggle the tab key moving focus. Alternatively, use esc then tab to move to the next interactive element on the page.
No file chosen
Attach files by dragging & dropping, selecting or pasting them.
Editing BOOLEAN_FUNCTION_MINIMIZATION/README.md at main · Yuvan2/BOOLEAN_FUNCTION_MINIMIZATION

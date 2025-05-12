# verilog-lab-1-building-a-multiplier-circuit-and-a-simple-calculator-solved
**TO GET THIS SOLUTION VISIT:** [Verilog Lab 1-Building a Multiplier Circuit and a Simple Calculator Solved](https://www.ankitcodinghub.com/product/verilog-lab-1-building-a-multiplier-circuit-and-a-simple-calculator-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91437&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Verilog Lab 1-Building a Multiplier Circuit and a Simple Calculator Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Lab 1

Building a Multiplier Circuit and a Simple Calculator

The purpose of this lab is to build a binary multiplier circuit, verify its functionality using a testbench, then combine it with an adder/subtractor circuit to create a basic calculator.

Part 1 (Building a multiplier circuit)

Two binary numbers can be multiplied in the same method used to multiply two decimal numbers. The figure below shows an example of multiplying 14×11=154. In this part, we focus on building an unsigned number multiplier, because signed number multiplication is more complex.

A binary multiplier can be implemented using several stages of full-adder (FA) blocks connected in a ripple-carry configuration. However, the delay caused by the carry signal rippling through the different FA blocks and the different stages can cause a significant impact on the time needed to generate a correct product result. The carry-save array configuration, is a binary multiplier that reduces the delay effect and produces correct results faster. The diagram below shows a 4-bit multiplier circuit arranged in a carry-save array configuration.

</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
In this part, you will build the carry-save array multiplier circuit shown in the figure above, then you will write a test bench to verify the functionality of your implmentation. In all your steps in this part, assume the numbers used are 4-bit unsigned integers.

The following steps should guide you through the implementation:

<ol>
<li>Verify the functionality of the circuit by tracing the multiplications 14×11 and 9×5
direclty on the digram. In other words, (with a pencil and paper) trace the patterns of 1’s and 0’s propagating through the different circuit elements, and verify they produce the correct results
</li>
<li>To reduce clutter and make your code easier to read, debug, and modify, you will use hierarchical design.</li>
<li>miqj can be simply implemented using a 2-input and gate. Write a verilog module (call it mq_4bit) that takes a 4-bit signal m, 1-bit signal q, and generates a 4-bit signal mq. Specifically, the module’s output should be anding the different bits of m with the signle bit of q. You might find the concatenation operator useful in this step</li>
<li>Import all files included with this guide. Open full_adder.v and make sure you understand how to use it.</li>
<li>Write a verilog module (call it csa_multiplier) to describe the circuit shown in the figure above. You should utilize the full_adder and mq_4bit modules and instantiate as many of them as necessary</li>
<li>Verify the functionality of csa_multiplier by writing a testbench (csa_multiplier_tb). You should use the following test vectors (0x10, 5×5, 9×5, 12×13, 15×10) to verify the multiplier is working correctly. You can add more test vectors if you want.</li>
<li>Include a screenshot of the simulation output with your submission, you might want to figure out how to embed it in your README.md file</li>
</ol>
Part 2 (Building a simple calculator)

In this part, you will combine the csa_multiplier and adder_subtractor (provided with this guide) to build a simple calculator. The calculator should perform 4-bit addition, subtraction, and multiplication. You will also verify the functionality of your calculator by implementing it on the FPGA board.

<ol>
<li>Write Verilog code to describe an 8-bit 2×1 multiplexer. This MUX will be used to control what is displayed at the output of the calculator</li>
<li>Write a Verilog module (simple_calc)

a. The module should accept two 4-bit inputs X, Y

b. The module should accept a 2-bit operator select input (op_sel).

i. op_sel = 00 (add)

ii. op_sel = 01 (subtract) iii. op_sel = 1x (multiply)

c. The module should output an 8-bit signal (result)
</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
<ol start="4">
<li>Draw a block diagram of the calculator. Show the different circuit elements and how they are connect. Specifically, your diagram should show a multiplier, adder/subtractor, and 8-bit 2×1 MUX circuit:
<ol>
<li>Instantiate an instance of a 4-bit adder/subtractor and connect X, Y and the appropriate add_n signal to it</li>
<li>Instantiate an instance of the 4-bit multiplier circuit you built in part 1. Connect X, Y to it</li>
<li>Instantiate an 8-bit 2×1 MUX you wrote in the step above. Connect the output of the multiplier to one input and the output of the adder/subtractor to the other input. You might also want to connect 4’b0 to the most significant bits of the input connected to the adder/subtractor.</li>
</ol>
</li>
<li>Verify the functionality of your simple calculator by implementing in on the FPGA board using the following IO specifications:
<ol>
<li>SW3ßSW0 for the inputX</li>
<li>SW7 ß SW4 for the input Y</li>
<li>SW15 ß SW14 for the op_sel</li>
<li>LED7 ß LED0 for the output result</li>
<li>LED14 to display the carry_out of the adder/subtractor</li>
<li>LED15 to display the overflow of the adder/subtractor</li>
</ol>
</li>
</ol>
</div>
</div>
</div>

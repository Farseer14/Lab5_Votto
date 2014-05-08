###ECE 281 

#####Lab5_Votto

#####Joseph Votto

Question: The file created instantiates a value of 8 which continues to increment through the four bit sequence until it reaches 0000 (overflow). It does this by using a counter (incrementing by 1 every iteration) and a jump programmed after the counter which continues to send the PC back to the counter. Finally, the program breaks out of the initial loop when the stored value reaches 0000 and proceeds to an infinite loop at the end.

Initial issues with this code include the apparent installation of the various sources. It took me until EI with Dr. Neebel to realize that I had multiple versions of the ALU and Datapath competing for dominance in the PRISM.

I just found out that my ALU was actually incorrect. When comparing the testbench to my simulation I found that it was not performing the add command. Dr. Neebel instructed me in correcting the issue and the TB and my simulation now match up.

I can't believe how far behind I am. I only just realized that I failed to retain how to insert component statements.

I am almost certain Dr. Neebel is getting aggrivated with my questions because I'm realizing that the next section of the directions usually includes references to the answers if not the answers themselves. And by the way, it appears as though the PRISM is now being implumented in the Nexus2_top_shell.

I feel like a child right now, I'm asking so many questions that I realize I should already know. I just need to remember where the directions for uploading the file to the FPGA is hiding.

Found Lab 1 back in the old archives, I'm heading back down for more EI. 

So the file generated, and doesn't appear to be working. After rooting around for a while it turned out that the only issues were an extrememly slow clock and an active low reset.

I'm sitting here just trying to understand how to start the Assembly segment of the program. 

So talking to C/Pluger about how to make a JN signal work to my advantage in this program, I was able to back track to what I need up to that point.

I can now add to the counter.

I based on the success with the incrementer, the decrement process should be working but continues to increment. Scratch that last. I was using the wrong import port to test. 

Questions:

1. All states 0

2. PCLd is asserted, next state is Direct IO Execute

3. IRLd, PCLd, and AddrSel are all passed

4. Given that the ACCL is being added to, the ACCLd must be active to retrieve the address

5. Unable to locate answer

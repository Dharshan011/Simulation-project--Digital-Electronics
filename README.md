## Design and simulate mod 3 synchronous counter using Verilog.

# AIM
Design and simulate mod 3 synchronous counter using Verilog.

## THEORY

Introduction: These types of counters fall under the category of synchronous controller counter. Here the mode control input is used to decide whether which sequence will be generated by the counter. In this case, mode control input is used to decide whether the counter will perform up counting or down counting In synchronous counter clock is provided to all the flip-flops simultaneously Circuit becomes complex as the number of states increases Speed is high

# PROGRAM

```
module mod3(input CLK,input reset,output[0:3]counter);
reg[0:3]counter_up;
always@(posedge CLK or posedge reset)
begin
if(reset)
counter_up<=4'd0;
else
counter_up<=counter_up+4'd1;
end
assign counter = counter_up;
endmodule
```

# PROGRAM INPUT
![Screenshot 2023-06-06 233204](https://github.com/Dharshan011/Simulation-project--Digital-Electronics/assets/113497491/81b0e600-a48d-49f6-bcca-40ec928b4115)




# LOGIC DIAGRAM


![Screenshot 2023-06-06 234310](https://github.com/Dharshan011/Simulation-project--Digital-Electronics/assets/113497491/d2627469-a28d-4680-93ef-50d6643edf35)


# TRUTH TABLE

![Screenshot 2023-06-06 234329](https://github.com/Dharshan011/Simulation-project--Digital-Electronics/assets/113497491/6ede0d68-db51-4812-843e-497fff865c9d)


## RTL DIAGRAM
![Screenshot 2023-06-06 233246](https://github.com/Dharshan011/Simulation-project--Digital-Electronics/assets/113497491/442e695a-4f39-4766-af11-49f17359a85f)


# TIMING DIAGRAM

![Screenshot 2023-06-06 233142](https://github.com/Dharshan011/Simulation-project--Digital-Electronics/assets/113497491/b03267eb-54cf-488a-b91d-14e4d1bdf1fd)

## RESULT
simulate mod 3 synchronous counter using Verilog is executed sucessfuly



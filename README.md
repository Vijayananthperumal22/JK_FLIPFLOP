# JK_FLIPFLOP
![image](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/154305926/094e9d55-5f30-4984-90b9-dd51d5297974)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/154305926/5b973ee8-9ee2-402d-8cba-1adfa2e4d5f2)
# Truth Table
![image](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/154305926/04d4ff52-ae20-4e08-bd70-58137b129890)
# Code
```
module jkff(clk,j,k,rst,q );
input j,k,clk,rst;
output reg q;
always@(posedge clk)
begin
if(rst==1)
q=1'b0;
else
begin
case({j,k})
2'b00: q=q;
2'b01:q=1'b0;
2'b10:q=1'b1;
2'b11:q=~q;
endcase
end
end
endmodule
```

# Output
![320401596-ce0a511a-b7b0-490b-8c74-eb759e6887ea](https://github.com/Vijayananthperumal22/JK_FLIPFLOP/assets/107705127/8b069d1d-2584-44a0-9a3d-43a2888b8a0f)

// verilog code for Half Adder in Data Flow Modeling

module halfadder(a,b,out,carry);
input a,b;
output out,carry;
assign = a^b;
assign =a&b;
endmodule

//Testbench


module halfadder_tb();
reg a,b;
wire a&b;
halfadder n1(a,b,out,carry);
initial begin
a=0; b=0;
#10 a=0; b=1;
#10 a=1; b=0;
#10 a=1; b=1;
#10 $stop
end
endmodule

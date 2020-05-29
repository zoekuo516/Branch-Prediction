# main()

## Input
entry_number >> entry number

Inst_history >> ASSEMBLY.txt

inst_counter 紀錄有幾行程式

## Output

//input: number of entries
8

entry: 2        beq R1,R2,End           //beq R1,R2,End 使用編號2的entry

(00, SN, SN, SN, SN) N N                misprediction: 0

//狀態            預測值 實際值            本預測器miss次數 (從頭統計至今)

entry: 4        beq R0,R0,Loop

(00, SN, SN, SN, SN) N T                misprediction: 1

entry: 2        beq R1,R2,End

(00, SN, SN, SN, SN) N N                misprediction: 0

entry: 4        beq R0,R0,Loop

(01, WN, SN, SN, SN) N T                misprediction: 2

entry: 2        beq R1,R2,End

(00, SN, SN, SN, SN) N N                misprediction: 0

entry: 4        beq R0,R0,Loop

(11, WN, WN, SN, SN) N T                misprediction: 3

entry: 2        beq R1,R2,End

(00, SN, SN, SN, SN) N N                misprediction: 0

entry: 4        beq R0,R0,Loop

(11, WN, WN, SN, WN) N T                misprediction: 4

entry: 2        beq R1,R2,End

(00, SN, SN, SN, SN) N T                misprediction: 1

# string_cut()

---字串處理---

# TBH_predict

根據history做出predict

根據predict與輸入的outcome判斷有沒有預測正確

更新History的值

根據outcome改變我們的Two Bit History

權重修正

# struct
## TBH
 ---Two Bit History---
 
 int history[2];
 
	int CNT[4];
	
	int mis_pre;
	
	vector<string> h
 
 ## Instruction
 string addr;
 
	string Type;
	
	int D_Reg;
	
	int InputA_Reg;
	
	int InputB_Reg;
	
	int immed;

	string D_Addr;
	
  ## Jump_Addr
  
  string addr;
  
	int inst_number;
	
	

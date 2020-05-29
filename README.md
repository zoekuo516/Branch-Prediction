# main()

## Input
entry_number >> entry number

Inst_history >> ASSEMBLY.txt

inst_counter 紀錄有幾行程式

## Output


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
	
	

# hw1_binary_hex_converter
def convert_number(decimal_number):
    binary_number = bin(decimal_number)[2:]  # 轉換為二進位並去掉前綴 '0b'
    hex_number = hex(decimal_number)[2:]  # 轉換為16進位並去掉前綴 '0x'
    
    return binary_number, hex_number

# 主程式
if __name__ == "__main__":
    try:
        decimal_input = int(input("請輸入10進位數字: "))
        binary_output, hex_output = convert_number(decimal_input)
        print(f"二進位: {binary_output}")
        print(f"16進位: {hex_output}")
    except ValueError:
        print("請輸入有效的整數！")


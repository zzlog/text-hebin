from collections import defaultdict

# 假设每行的格式是：账号,数据
def process_file(input_file, output_file):
    account_data = defaultdict(list)

    # 读取文件并将相同账号的数据合并
    with open(input_file, 'r') as file:
        for line in file:
            account, data = line.strip().split(',')
            account_data[account].append(data)

    # 将合并后的数据写入输出文件
    with open(output_file, 'w') as file:
        for account, data_list in account_data.items():
            combined_data = ','.join(data_list)
            file.write(f"{account},{combined_data}\n")

# 示例调用
input_file = 'input.txt'  # 输入文件名
output_file = 'output.txt'  # 输出文件名
process_file(input_file, output_file)

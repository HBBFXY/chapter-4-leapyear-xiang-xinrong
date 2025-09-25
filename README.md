def is_leap_year(year):
    """判断是否为闰年"""
    return (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0)

def main():
    try:
        year = int(input("请输入年份："))
        if is_leap_year(year):
            print(f"{year}是闰年")
        else:
            print(f"{year}不是闰年")
    except ValueError:
        print("输入错误，请输入有效的年份数字")

if __name__ == "__main__":
    main()

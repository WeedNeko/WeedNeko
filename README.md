import requests

# Nhập khóa API của bạn
api_key = 141411

# Tạo một đối tượng requests
session = requests.Session()

# Xác thực với GitRob
session.auth = (api_key, "")

# Thực hiện một yêu cầu
response = session.get("https://api.gitrob.com/repos/")

# In kết quả
print(response.json())

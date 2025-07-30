local HttpService = game:GetService("HttpService")

-- Thay bằng webhook của bạn
local webhook_url = "https://canary.discord.com/api/webhooks/1400014470365052948/-oOD2uRSpvSJVC3FPUtqm1W_PSS8VvH7CcrrFsVTAa8WX9yMojPRa-aSZcWIbMUcqUXw"

-- Câu hỏi người chơi nhập
local user_input = "game này có script auto nào không?"

local data = {
    ["content"] = user_input
}

local jsonData = HttpService:JSONEncode(data)

local response = syn.request({
    Url = webhook_url,
    Method = "POST",
    Headers = {
        ["Content-Type"] = "application/json"
    },
    Body = jsonData
})

print("Đã gửi câu hỏi đến webhook")

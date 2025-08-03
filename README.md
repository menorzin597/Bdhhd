
getgenv().autoThank = true --u can change this
msgsTable = {
"master oogway thanks u",-- u can change this
"fr fr omg ty",--u can change this
"me when the impostor donated, thanks",--u can change this
"lets goo dude thanks"--u can change this
}
game.Players.LocalPlayer.leaderstats.Raised.Changed:Connect(function()
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(msgsTable[math.random(0, #msgsTable)], "all")
end)
local VirtualUser= game:GetService("VirtualUser")
game.Players.LocalPlayer.Idled:connect(function()
VirtualUser:CaptureController()
VirtualUser:ClickButton2(Vector2.new())
end)

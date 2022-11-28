local JNHHGaming = Instance.new("ScreenGui")

local TextLabel = Instance.new("TextButton")

local UIGradient = Instance.new("UIGradient")

local TextLabel_2 = Instance.new("TextLabel")

local UIGradient_2 = Instance.new("UIGradient")

local UITextSizeConstraint = Instance.new("UITextSizeConstraint")

local UITextSizeConstraint_2 = Instance.new("UITextSizeConstraint")

JNHHGaming.Name = "JNHHGaming"

JNHHGaming.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

JNHHGaming.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

JNHHGaming.ResetOnSpawn = false

TextLabel.Parent = JNHHGaming

TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)

TextLabel.BackgroundTransparency = 1.000

TextLabel.BorderSizePixel = 0

TextLabel.Position = UDim2.new(-0.000772226602, 0, 0.0343558267, 0)

TextLabel.Size = UDim2.new(0.180134634, 0, 0.0800389072, 0)

TextLabel.Font = Enum.Font.GothamBold

TextLabel.Text = "kill aura v1"

TextLabel.TextColor3 = Color3.fromRGB(255,0,0)

TextLabel.TextScaled = true

TextLabel.TextSize = 28.000

TextLabel.TextWrapped = true

TextLabel.TextXAlignment = Enum.TextXAlignment.Left

TextLabel.MouseButton1Down:Connect(function()

	while true do wait() game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 23.3 endWalkspeed()

end)

UIGradient.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(126, 0, 0)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(209, 0, 0))}

UIGradient.Parent = TextLabel

TextLabel_2.Parent = TextLabel

TextLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)

TextLabel_2.BackgroundTransparency = 1.000

TextLabel_2.BorderSizePixel = 0

TextLabel_2.Position = UDim2.new(-0.000772226602, 0, 0.77410934, 0)

TextLabel_2.Size = UDim2.new(1.2, 0, 1.2, 0)

TextLabel_2.Font = Enum.Font.GothamBold

TextLabel_2.Text = "Kill AURA ACTIVATED"

TextLabel_2.TextColor3 = Color3.fromRGB(1,1,1)

TextLabel_2.TextScaled = true

TextLabel_2.TextSize = 24.000

TextLabel_2.TextWrapped = true

TextLabel_2.TextXAlignment = Enum.TextXAlignment.Left

UIGradient_2.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(126, 0, 0)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(209, 0, 0))}

UIGradient_2.Parent = TextLabel_2

UITextSizeConstraint.Parent = TextLabel_2

UITextSizeConstraint.MaxTextSize = 24

UITextSizeConstraint_2.Parent = TextLabel

UITextSizeConstraint_2.MaxTextSize = 27

local vu = game:GetService("VirtualUser")

game:GetService("Players").LocalPlayer.Idled:connect(function()

    vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)

    wait(1)

    vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)

end)

local vu = game:GetService("VirtualUser")

game:GetService("Players").LocalPlayer.Idled:connect(function()

    vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)

    wait(1)

    vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)

end)

 

game.StarterGui:SetCore("SendNotification", {

    Title = "Bedwars Temporary Script";

    Text = "Made by JN HH Gaming and Monia"; -- what the text says (ofc)

    Duration = 15;

})

wait(1)

game.StarterGui:SetCore("SendNotification", {

    Title = "Enjoy";

    Text = "Don't Forget to Subscribe JN HH Gaming"; -- what the text says (ofc)

    Duration = 30;

})

wait(1)

game.StarterGui:SetCore("SendNotification", {

    Title = " Also Join NightBed Discord";

    Text = "https://discord.gg/k7zj7yfCrx"; -- what the text says (ofc)

    Duration = 30;

})

-- Gui to Lua

-- Version: 3.

-- Instances:

local ScreenGui = Instance.new("ScreenGui")

local Main = Instance.new("Frame")

local TextLabel = Instance.new("TextLabel")

local TextButton = Instance.new("TextButton")

--Properties:

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

Main.Name = "Main"

Main.Parent = ScreenGui

Main.BackgroundColor3 = Color3.fromRGB(39, 15, 245)

Main.Position = UDim2.new(0.363293529, 0, 0.28638497, 0)

Main.Size = UDim2.new(0, 300, 0, 154)

Main.Style = Enum.FrameStyle.ChatRed

TextLabel.Parent = Main

TextLabel.BackgroundColor3 = Color3.fromRGB(17, 1, 1)

TextLabel.BackgroundTransparency = 1.000

TextLabel.Position = UDim2.new(-0.025588274, 0, -0.0890700519, 0)

TextLabel.Size = UDim2.new(0, 250, 0, 30)

TextLabel.Font = Enum.Font.SciFi

TextLabel.Text = "Kill Aura "

TextLabel.TextColor3 = Color3.fromRGB(245, 16, 16)

TextLabel.TextScaled = true

TextLabel.TextSize = 12.000

TextLabel.TextWrapped = true

TextButton.Parent = Main

TextButton.BackgroundColor3 = Color3.fromRGB(17, 1, 1)

TextButton.Position = UDim2.new(0.136470661, 0, 0.458670378, 0)

TextButton.Size = UDim2.new(0, 200, 0, 58)

TextButton.Style = Enum.ButtonStyle.RobloxRoundDefaultButton

TextButton.Font = Enum.Font.SciFi

TextButton.Text = "Click To Activate"

TextButton.TextColor3 = Color3.fromRGB(21, 235, 78)

TextButton.TextScaled = true

TextButton.TextSize = 14.000

TextButton.TextWrapped = true

TextButton.MouseButton1Down:connect(function()

 while true do 
 
 wait() 
 
 local player = game:GetService("Players")

local lplr = player.LocalPlayer

local cam = workspace.CurrentCamera

local KnitClient = debug.getupvalue(require(lplr.PlayerScripts.TS.knit).setup, 6)

local SwordCont = KnitClient.Controllers.SwordController

local aura = false

local DistVal = {["Value"] = 14}

function Aura()

	for i,v in pairs(game.Players:GetChildren()) do

		if v.Character and v.Name ~= game.Players.LocalPlayer.Name and v.Character:FindFirstChild("HumanoidRootPart") then

			local mag = (v.Character.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude

			if mag <= DistVal["Value"] and v.Team ~= game.Players.LocalPlayer.Team and v.Character:FindFirstChild("Humanoid") then

				if v.Character.Humanoid.Health > 0 then

					aura = true

                    SwordCont:swingSwordAtMouse()

end

end

end

end

end

game:GetService("RunService").Stepped:connect(function()

Aura()

end)

end)

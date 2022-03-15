-- Gui to Lua
-- Version: 3.2

-- Instances:

local RandomChooser = Instance.new("ScreenGui")
local Menu = Instance.new("Frame")
local Titile = Instance.new("TextLabel")
local Corner = Instance.new("UICorner")
local Corner_2 = Instance.new("UICorner")
local Title = Instance.new("TextLabel")
local MeUserName = Instance.new("TextLabel")
local Start = Instance.new("TextButton")
local Frame = Instance.new("Frame")
local PlayersListBut = Instance.new("TextButton")
local ParticipantsButton = Instance.new("TextButton")
local PgTitle = Instance.new("TextLabel")
local Participants = Instance.new("Frame")
local ParticipantsFrame = Instance.new("ScrollingFrame")
local Template = Instance.new("Frame")
local PlayerAvatar = Instance.new("ImageLabel")
local PlayerName = Instance.new("TextLabel")
local UIGridLayout = Instance.new("UIGridLayout")
local Search = Instance.new("TextBox")
local AddAll = Instance.new("TextButton")
local Clear = Instance.new("TextButton")
local PlayerLissssss = Instance.new("Frame")
local PlayerList = Instance.new("ScrollingFrame")
local UIGridLayout_2 = Instance.new("UIGridLayout")
local Template_2 = Instance.new("Frame")
local PlayerAvatar_2 = Instance.new("ImageLabel")
local PlayerName_2 = Instance.new("TextLabel")
local StartChoosing = Instance.new("TextButton")
local WinnerFrame = Instance.new("Frame")
local Close = Instance.new("TextButton")
local Send = Instance.new("TextButton")
local Remove = Instance.new("TextButton")
local WinnerTitle = Instance.new("TextLabel")
local WinerAvatar = Instance.new("ImageLabel")
local WinnerName = Instance.new("TextLabel")
local Players = game.Players
local ParticipantsNumber = 0
local Can = false
local Can1 = false
local Can2 = false
local Ready = false
local Ready1 = false

--Properties:

RandomChooser.Name = "RandomChooser"
RandomChooser.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
RandomChooser.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Menu.Name = "Menu"
Menu.Parent = RandomChooser
Menu.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Menu.BackgroundTransparency = 0.400
Menu.Position = UDim2.new(0.340442985, 0, 0.333689809, 0)
Menu.Size = UDim2.new(0, 388, 0, 310)

Titile.Name = "Titile"
Titile.Parent = Menu
Titile.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Titile.BackgroundTransparency = 0.500
Titile.Size = UDim2.new(0, 388, 0, 50)
Titile.Font = Enum.Font.FredokaOne
Titile.Text = "Random Chooser"
Titile.TextColor3 = Color3.fromRGB(85, 255, 127)
Titile.TextScaled = true
Titile.TextSize = 14.000
Titile.TextWrapped = true

Corner.CornerRadius = UDim.new(0, 13)
Corner.Name = "Corner"
Corner.Parent = Titile

Corner_2.CornerRadius = UDim.new(0, 13)
Corner_2.Name = "Corner"
Corner_2.Parent = Menu

Title.Name = "Title"
Title.Parent = Menu
Title.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Title.BackgroundTransparency = 1.000
Title.Position = UDim2.new(0.0824742243, 0, 0.290322572, 0)
Title.Size = UDim2.new(0, 324, 0, 50)
Title.Font = Enum.Font.FredokaOne
Title.Text = "Thanks for using,"
Title.TextColor3 = Color3.fromRGB(255, 255, 255)
Title.TextScaled = true
Title.TextSize = 14.000
Title.TextWrapped = true

MeUserName.Name = "MeUserName"
MeUserName.Parent = Menu
MeUserName.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
MeUserName.BackgroundTransparency = 1.000
MeUserName.Position = UDim2.new(0.211340204, 0, 0.45161289, 0)
MeUserName.Size = UDim2.new(0, 224, 0, 43)
MeUserName.Font = Enum.Font.FredokaOne
MeUserName.Text = "Roblox_Wmh"
MeUserName.TextColor3 = Color3.fromRGB(255, 170, 0)
MeUserName.TextScaled = true
MeUserName.TextSize = 14.000
MeUserName.TextWrapped = true
MeUserName.Text = game.Players.LocalPlayer.Name

Start.Name = "Start"
Start.Parent = Menu
Start.BackgroundColor3 = Color3.fromRGB(76, 76, 76)
Start.BackgroundTransparency = 0.400
Start.Position = UDim2.new(0.242268041, 0, 0.719354868, 0)
Start.Size = UDim2.new(0, 200, 0, 50)
Start.Font = Enum.Font.FredokaOne
Start.Text = "Start"
Start.TextColor3 = Color3.fromRGB(85, 255, 0)
Start.TextScaled = true
Start.TextSize = 14.000
Start.TextWrapped = true

Frame.Parent = RandomChooser
Frame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Frame.BackgroundTransparency = 0.400
Frame.BorderColor3 = Color3.fromRGB(72, 72, 72)
Frame.BorderSizePixel = 3
Frame.Position = UDim2.new(0.261689901, 0, 0.270588219, 0)
Frame.Size = UDim2.new(0, 580, 0, 428)
Frame.Visible = false

PlayersListBut.Name = "PlayersListBut"
PlayersListBut.Parent = Frame
PlayersListBut.BackgroundColor3 = Color3.fromRGB(135, 135, 135)
PlayersListBut.BackgroundTransparency = 0.600
PlayersListBut.BorderSizePixel = 3
PlayersListBut.Position = UDim2.new(0.675454378, 0, 0.870519042, 0)
PlayersListBut.Size = UDim2.new(0, 187, 0, 54)
PlayersListBut.Font = Enum.Font.FredokaOne
PlayersListBut.Text = "Players"
PlayersListBut.TextColor3 = Color3.fromRGB(85, 170, 255)
PlayersListBut.TextScaled = true
PlayersListBut.TextSize = 14.000
PlayersListBut.TextWrapped = true

ParticipantsButton.Name = "ParticipantsButton"
ParticipantsButton.Parent = Frame
ParticipantsButton.BackgroundColor3 = Color3.fromRGB(135, 135, 135)
ParticipantsButton.BackgroundTransparency = 0.600
ParticipantsButton.BorderSizePixel = 3
ParticipantsButton.Position = UDim2.new(0.00308822095, 0, 0.870519042, 0)
ParticipantsButton.Size = UDim2.new(0, 187, 0, 54)
ParticipantsButton.Font = Enum.Font.FredokaOne
ParticipantsButton.Text = "Participants"
ParticipantsButton.TextColor3 = Color3.fromRGB(85, 170, 255)
ParticipantsButton.TextScaled = true
ParticipantsButton.TextSize = 14.000
ParticipantsButton.TextWrapped = true

PgTitle.Name = "PgTitle"
PgTitle.Parent = Frame
PgTitle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
PgTitle.BackgroundTransparency = 1.000
PgTitle.Position = UDim2.new(0.00258620689, 0, 0.00350467279, 0)
PgTitle.Size = UDim2.new(0, 577, 0, 50)
PgTitle.Font = Enum.Font.FredokaOne
PgTitle.Text = "Chooser"
PgTitle.TextColor3 = Color3.fromRGB(85, 255, 127)
PgTitle.TextScaled = true
PgTitle.TextSize = 14.000
PgTitle.TextWrapped = true

Participants.Name = "Participants"
Participants.Parent = Frame
Participants.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Participants.BackgroundTransparency = 1.000
Participants.BorderColor3 = Color3.fromRGB(107, 107, 107)
Participants.BorderSizePixel = 3
Participants.Position = UDim2.new(0.0853740796, 0, 0.122379407, 0)
Participants.Size = UDim2.new(0, 469, 0, 275)
Participants.Visible = false

ParticipantsFrame.Name = "ParticipantsFrame"
ParticipantsFrame.Parent = Participants
ParticipantsFrame.Active = true
ParticipantsFrame.BackgroundColor3 = Color3.fromRGB(63, 63, 63)
ParticipantsFrame.BackgroundTransparency = 0.300
ParticipantsFrame.BorderColor3 = Color3.fromRGB(4, 4, 4)
ParticipantsFrame.BorderSizePixel = 3
ParticipantsFrame.Position = UDim2.new(-0.000380198151, 0, -0.000922740612, 0)
ParticipantsFrame.Size = UDim2.new(0, 480, 0, 230)
ParticipantsFrame.ScrollBarThickness = 10

Template.Name = "Template"
Template.Parent = ParticipantsFrame
Template.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Template.Position = UDim2.new(-0.00421552965, 0, -0.00363636366, 0)
Template.Size = UDim2.new(0, 117, 0, 100)
Template.Visible = false

PlayerAvatar.Name = "PlayerAvatar"
PlayerAvatar.Parent = Template
PlayerAvatar.BackgroundColor3 = Color3.fromRGB(85, 255, 255)
PlayerAvatar.BackgroundTransparency = 1.000
PlayerAvatar.Size = UDim2.new(0, 117, 0, 68)
PlayerAvatar.Image = "http://www.roblox.com/asset/?id=5365990711"

PlayerName.Name = "PlayerName"
PlayerName.Parent = Template
PlayerName.BackgroundColor3 = Color3.fromRGB(56, 56, 56)
PlayerName.BackgroundTransparency = 0.200
PlayerName.Position = UDim2.new(0, 0, 0.680000007, 0)
PlayerName.Size = UDim2.new(0, 117, 0, 32)
PlayerName.Font = Enum.Font.FredokaOne
PlayerName.Text = "Roblox_Wmh"
PlayerName.TextColor3 = Color3.fromRGB(255, 255, 127)
PlayerName.TextScaled = true
PlayerName.TextSize = 14.000
PlayerName.TextWrapped = true

UIGridLayout.Parent = ParticipantsFrame
UIGridLayout.SortOrder = Enum.SortOrder.LayoutOrder
UIGridLayout.CellPadding = UDim2.new(0, 0, 0, 0)
UIGridLayout.CellSize = UDim2.new(0, 117, 0, 100)

Search.Name = "Search"
Search.Parent = Participants
Search.BackgroundColor3 = Color3.fromRGB(104, 104, 104)
Search.BorderSizePixel = 3
Search.Position = UDim2.new(0.329608321, 0, 0.847854972, 0)
Search.Size = UDim2.new(0, 157, 0, 44)
Search.Font = Enum.Font.FredokaOne
Search.Text = ""
Search.TextColor3 = Color3.fromRGB(33, 66, 49)
Search.TextScaled = true
Search.TextSize = 14.000
Search.TextWrapped = true

AddAll.Name = "AddAll"
AddAll.Parent = Participants
AddAll.BackgroundColor3 = Color3.fromRGB(61, 61, 61)
AddAll.BackgroundTransparency = 0.300
AddAll.BorderSizePixel = 3
AddAll.Position = UDim2.new(-0.00531682558, 0, 0.844541788, 0)
AddAll.Size = UDim2.new(0, 156, 0, 46)
AddAll.Font = Enum.Font.FredokaOne
AddAll.Text = "Add All"
AddAll.TextColor3 = Color3.fromRGB(255, 170, 0)
AddAll.TextScaled = true
AddAll.TextSize = 14.000
AddAll.TextWrapped = true

Clear.Name = "Clear"
Clear.Parent = Participants
Clear.BackgroundColor3 = Color3.fromRGB(61, 61, 61)
Clear.BackgroundTransparency = 0.300
Clear.BorderSizePixel = 3
Clear.Position = UDim2.new(0.666324973, 0, 0.844541788, 0)
Clear.Size = UDim2.new(0, 156, 0, 46)
Clear.Font = Enum.Font.FredokaOne
Clear.Text = "Clear"
Clear.TextColor3 = Color3.fromRGB(255, 170, 0)
Clear.TextScaled = true
Clear.TextSize = 14.000
Clear.TextWrapped = true

PlayerLissssss.Name = "PlayerLissssss"
PlayerLissssss.Parent = Frame
PlayerLissssss.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
PlayerLissssss.BackgroundTransparency = 1.000
PlayerLissssss.BorderColor3 = Color3.fromRGB(107, 107, 107)
PlayerLissssss.BorderSizePixel = 3
PlayerLissssss.Position = UDim2.new(0.0853740796, 0, 0.122379407, 0)
PlayerLissssss.Size = UDim2.new(0, 469, 0, 275)
PlayerLissssss.Visible = false

PlayerList.Name = "PlayerList"
PlayerList.Parent = PlayerLissssss
PlayerList.Active = true
PlayerList.BackgroundColor3 = Color3.fromRGB(63, 63, 63)
PlayerList.BackgroundTransparency = 0.300
PlayerList.BorderColor3 = Color3.fromRGB(4, 4, 4)
PlayerList.BorderSizePixel = 3
PlayerList.Position = UDim2.new(0.00282050087, 0, 0.00454190327, 0)
PlayerList.Size = UDim2.new(0, 480, 0, 270)
PlayerList.CanvasPosition = Vector2.new(0, 273.999969)
PlayerList.ScrollBarThickness = 10

UIGridLayout_2.Parent = PlayerList
UIGridLayout_2.SortOrder = Enum.SortOrder.LayoutOrder
UIGridLayout_2.CellPadding = UDim2.new(0, 0, 0, 0)
UIGridLayout_2.CellSize = UDim2.new(0, 117, 0, 100)

Template_2.Name = "Template"
Template_2.Parent = PlayerList
Template_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Template_2.Position = UDim2.new(-0.00421552965, 0, -0.00363636366, 0)
Template_2.Size = UDim2.new(0, 117, 0, 100)
Template_2.Visible = false

PlayerAvatar_2.Name = "PlayerAvatar"
PlayerAvatar_2.Parent = Template_2
PlayerAvatar_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
PlayerAvatar_2.BackgroundTransparency = 1.000
PlayerAvatar_2.Size = UDim2.new(0, 117, 0, 68)
PlayerAvatar_2.Image = "rbxasset://textures/ui/GuiImagePlaceholder.png"

PlayerName_2.Name = "PlayerName"
PlayerName_2.Parent = Template_2
PlayerName_2.BackgroundColor3 = Color3.fromRGB(56, 56, 56)
PlayerName_2.BackgroundTransparency = 0.200
PlayerName_2.Position = UDim2.new(0, 0, 0.680000007, 0)
PlayerName_2.Size = UDim2.new(0, 117, 0, 32)
PlayerName_2.Font = Enum.Font.FredokaOne
PlayerName_2.Text = "Roblox_Wmh"
PlayerName_2.TextColor3 = Color3.fromRGB(255, 255, 127)
PlayerName_2.TextScaled = true
PlayerName_2.TextSize = 14.000
PlayerName_2.TextWrapped = true

StartChoosing.Name = "StartChoosing"
StartChoosing.Parent = Frame
StartChoosing.BackgroundColor3 = Color3.fromRGB(135, 135, 135)
StartChoosing.BackgroundTransparency = 0.600
StartChoosing.BorderColor3 = Color3.fromRGB(85, 255, 127)
StartChoosing.BorderSizePixel = 3
StartChoosing.Position = UDim2.new(0.273557693, 0, 0.409223765, 0)
StartChoosing.Size = UDim2.new(0, 261, 0, 63)
StartChoosing.Font = Enum.Font.FredokaOne
StartChoosing.Text = "Start Choosing"
StartChoosing.TextColor3 = Color3.fromRGB(255, 85, 0)
StartChoosing.TextScaled = true
StartChoosing.TextSize = 14.000
StartChoosing.TextWrapped = true

WinnerFrame.Name = "WinnerFrame"
WinnerFrame.Parent = Frame
WinnerFrame.BackgroundColor3 = Color3.fromRGB(13, 13, 13)
WinnerFrame.Position = UDim2.new(0.275067866, 0, 0.20988892, 0)
WinnerFrame.Size = UDim2.new(0, 270, 0, 226)
WinnerFrame.Visible = false

Close.Name = "Close"
Close.Parent = WinnerFrame
Close.BackgroundColor3 = Color3.fromRGB(12, 12, 12)
Close.BackgroundTransparency = 0.100
Close.BorderSizePixel = 3
Close.Position = UDim2.new(-0.00370370364, 0, 0.774336159, 0)
Close.Size = UDim2.new(0, 90, 0, 50)
Close.Font = Enum.Font.FredokaOne
Close.Text = "Close"
Close.TextColor3 = Color3.fromRGB(255, 255, 127)
Close.TextScaled = true
Close.TextSize = 14.000
Close.TextWrapped = true

Send.Name = "Send"
Send.Parent = WinnerFrame
Send.BackgroundColor3 = Color3.fromRGB(12, 12, 12)
Send.BackgroundTransparency = 0.100
Send.BorderSizePixel = 3
Send.Position = UDim2.new(0.333333313, 0, 0.774336159, 0)
Send.Size = UDim2.new(0, 90, 0, 50)
Send.Font = Enum.Font.FredokaOne
Send.Text = "Send to chat"
Send.TextColor3 = Color3.fromRGB(255, 255, 127)
Send.TextScaled = true
Send.TextSize = 14.000
Send.TextWrapped = true

Remove.Name = "Remove"
Remove.Parent = WinnerFrame
Remove.BackgroundColor3 = Color3.fromRGB(12, 12, 12)
Remove.BackgroundTransparency = 0.100
Remove.BorderSizePixel = 3
Remove.Position = UDim2.new(0.666666627, 0, 0.774336159, 0)
Remove.Size = UDim2.new(0, 90, 0, 50)
Remove.Font = Enum.Font.FredokaOne
Remove.Text = "Remove"
Remove.TextColor3 = Color3.fromRGB(255, 255, 127)
Remove.TextScaled = true
Remove.TextSize = 14.000
Remove.TextWrapped = true

WinnerTitle.Name = "WinnerTitle"
WinnerTitle.Parent = WinnerFrame
WinnerTitle.BackgroundColor3 = Color3.fromRGB(12, 12, 12)
WinnerTitle.BackgroundTransparency = 0.100
WinnerTitle.Position = UDim2.new(-0.00370370364, 0, 0, 0)
WinnerTitle.Size = UDim2.new(0, 271, 0, 50)
WinnerTitle.Font = Enum.Font.FredokaOne
WinnerTitle.Text = "Winner Is:"
WinnerTitle.TextColor3 = Color3.fromRGB(85, 255, 0)
WinnerTitle.TextScaled = true
WinnerTitle.TextSize = 14.000
WinnerTitle.TextWrapped = true

WinerAvatar.Name = "WinerAvatar"
WinerAvatar.Parent = WinnerFrame
WinerAvatar.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
WinerAvatar.BackgroundTransparency = 1.000
WinerAvatar.Position = UDim2.new(0.311111122, 0, 0.221238941, 0)
WinerAvatar.Size = UDim2.new(0, 100, 0, 89)
WinerAvatar.Image = "rbxasset://textures/ui/GuiImagePlaceholder.png"

WinnerName.Name = "WinnerName"
WinnerName.Parent = WinnerFrame
WinnerName.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
WinnerName.Position = UDim2.new(0.129629627, 0, 0.623893797, 0)
WinnerName.Size = UDim2.new(0, 200, 0, 34)
WinnerName.Font = Enum.Font.FredokaOne
WinnerName.Text = "Roblox_Wmh"
WinnerName.TextColor3 = Color3.fromRGB(255, 255, 255)
WinnerName.TextScaled = true
WinnerName.TextSize = 14.000
WinnerName.TextWrapped = true

Start.MouseButton1Click:Connect(function()
	if Can == false then
		Can = true
		Frame.Visible = true
		Menu.Visible = false
	end
end)

ParticipantsButton.MouseButton1Click:Connect(function()
	if Can1 == false and PlayerLissssss.Visible == false and WinnerFrame.Visible == false then
		Can1 = true
		Participants.Visible = true
		StartChoosing.Visible = false
		while wait() do
			if Participants.Visible == true then
				PgTitle.Text = "Participants ".. ParticipantsNumber .."/20"
			end
		end
	else
		if Can1 == true then
			Can1 = false
			Participants.Visible = false
			StartChoosing.Visible = true
			PgTitle.Text = "Chooser"
		end
	end
end)

PlayersListBut.MouseButton1Click:Connect(function()
	if Can2 == false and Participants.Visible == false and WinnerFrame.Visible == false  then
		Can2 = true
		PlayerLissssss.Visible = true
		StartChoosing.Visible = false
		while wait() do
			if PlayerLissssss.Visible == true then
				PgTitle.Text = "Players ".. game.Players.NumPlayers .. "/" .. game.Players.MaxPlayers
			end
		end
	else
		if Can2 == true then
			Can2 = false
			PlayerLissssss.Visible = false
			StartChoosing.Visible = true
			PgTitle.Text = "Chooser"
		end
	end
end)



AddAll.MouseButton1Click:Connect(function()
	for i,v in pairs(game.Players:GetChildren()) do
		if ParticipantsFrame:FindFirstChild(v.Name) or ParticipantsNumber >= 20 then
			print("Got1")
		else
			Template:Destroy()
			local Template = Template:Clone()
			local Avatar = PlayerAvatar:Clone()
			local PlayerUserName = PlayerName:Clone()
			Template.Parent = ParticipantsFrame
			Template.Visible = true
			Template.Name = v.Name
			Template.BackgroundTransparency = 1
			Avatar.Parent = Template
			Avatar.Image = game.Players:GetUserThumbnailAsync(v.UserId, Enum.ThumbnailType.AvatarThumbnail, Enum.ThumbnailSize.Size420x420)
			Avatar.BackgroundTransparency = 1.000
			PlayerUserName.Text = v.Name
			PlayerUserName.Parent = Template
			ParticipantsNumber +=1
		end
	end
end)

Clear.MouseButton1Click:Connect(function()
	for i,v in pairs(ParticipantsFrame:GetChildren()) do
		if v:IsA("Frame") then
			v:Destroy()
			ParticipantsNumber = 0
		end
	end
end)

Search.Changed:Connect(function()
	for i,v in pairs(game.Players:GetChildren()) do
		if v.Name == Search.Text then
			if ParticipantsFrame:FindFirstChild(v.Name) or ParticipantsNumber >= 20 then
				print("Got")
			else
				Template:Destroy()
				local Template = Template:Clone()
				local Avatar = PlayerAvatar:Clone()
				local PlayerUserName = PlayerName:Clone()
				Template.Parent = ParticipantsFrame
				Template.Visible = true
				Template.Name = v.Name
				Template.BackgroundTransparency = 1
				Avatar.Parent = Template
				Avatar.Image = game.Players:GetUserThumbnailAsync(v.UserId, Enum.ThumbnailType.AvatarThumbnail, Enum.ThumbnailSize.Size420x420)
				Avatar.BackgroundTransparency = 1.000
				PlayerUserName.Text = v.Name
				PlayerUserName.Parent = Template
				ParticipantsNumber +=1
			end
		end
	end
end)

StartChoosing.MouseButton1Click:Connect(function()
	if Ready == false then
		Ready = true
		if ParticipantsNumber == 1 then
			StartChoosing.Text = ".."
			wait(0.05)
			StartChoosing.Text = "."
			wait(0.05)
			StartChoosing.Text = ".."
			wait(0.05)
			StartChoosing.Text = "."
			wait(0.05)
			StartChoosing.Text = ".."
			wait(0.05)
			StartChoosing.Text = "."
			wait(0.05)
			StartChoosing.Text = ".."
			wait(0.05)
			StartChoosing.Text = "."
			wait(1)
			local Win = ParticipantsFrame:GetChildren()
			local Winner = Win[math.random(1, #Win)]
			StartChoosing.Text = Winner.Name
			WinnerFrame.Visible = true
			Ready = false
			StartChoosing.Visible = false
			StartChoosing.Text = "StartChoosing"
			for i,v in pairs(game.Players:GetChildren()) do
				if v.Name == Winner.Name then
					WinnerName.Text = Winner.Name
					WinerAvatar.Visible = true
					WinerAvatar.Image = game.Players:GetUserThumbnailAsync(v.UserId, Enum.ThumbnailType.AvatarThumbnail, Enum.ThumbnailSize.Size420x420)
				else
					WinnerName.Text = "Nobody"
					WinerAvatar.Visible = false
				end
			end
		else
			StartChoosing.Text = "You need at least 2 players to choose"
			wait(2)
			StartChoosing.Text = "Start Choosing"
			wait(1)
			Ready = false
		end
	end
end)

Close.MouseButton1Click:Connect(function()
	if WinnerFrame.Visible == true then
		StartChoosing.Visible = true
		WinnerFrame.Visible = false
		Ready = false
	end
end)

Send.MouseButton1Click:Connect(function()
	game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("The winner is ".. WinnerName.Text, "All")
end)

Remove.MouseButton1Click:Connect(function()
	for i,v in pairs(game.Players:GetChildren()) do
		if v.Name == WinnerName.Text then
			ParticipantsFrame:FindFirstChild(WinnerName.Text):Destroy()
			ParticipantsNumber -= 1
			WinnerFrame.Visible = false
			StartChoosing.Visible = true
		else
			WinnerFrame.Visible = false
			StartChoosing.Visible = true
		end
	end
end)

function ClearUp()
	for i,a in pairs(PlayerList:GetChildren()) do
		if a:IsA("Frame") then
			a:Destroy()
		end
	end
end

function FillUp()
	ClearUp()
	for i,v in pairs(game.Players:GetChildren()) do
		if v:FindFirstChild(v.Name) then
		else
			Template:Destroy()
			local Template = Template:Clone()
			local Avatar = PlayerAvatar:Clone()
			local PlayerUserName = PlayerName:Clone()
			Template.Parent = PlayerList
			Template.Visible = true
			Template.Name = v.Name
			Template.BackgroundTransparency = 1
			Avatar.Parent = Template
			Avatar.Image = game.Players:GetUserThumbnailAsync(v.UserId, Enum.ThumbnailType.AvatarThumbnail, Enum.ThumbnailSize.Size420x420)
			Avatar.BackgroundTransparency = 1.000
			PlayerUserName.Text = v.Name
			PlayerUserName.Parent = Template
		end
	end
end

FillUp()

while wait(0.3) do
	FillUp()
end


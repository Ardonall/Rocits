 while true do wait()
 local buh = "Leisure"
 local bruh = {
  ["Name"] = "Gift",
  ["Amount"] = 1
  
  }
 
 


Workspace.CommunicationRelays.Transaction.ConsumeItem:InvokeServer(buh, bruh)
 

 local descendants = game.Players.LocalPlayer.PlayerGui.Inventory.Container.List.Furniture:GetDescendants()
    local lol = game.workspace:GetDescendants()

 for index, descendants in pairs(descendants) do 
  if descendants .Name == "ColorOptions" then 

   
local ohString1 = "Furniture"
local ohTable2 = {
 ["Serial"] = descendants.Parent.Name
}

workspace.CommunicationRelays.Transaction.SellItem:InvokeServer(ohString1, ohTable2)
   
   end
  end
 end

# Creating a Land Claim

In TnologyMC, you can create land claims in order to protect your land. To create a claim, you will need a Golden Shovel. You get a golden shovel upon joining, and can get one from `/kit default`.

Note that you will only have 500 land claim blocks when you first join. This is to prevent new players creating large claims that they don't need. You get more claim blocks by playing on the server more, and can earn claim blocks via crates.

To start, hold the golden shovel and right click the first corner block of the claim area you want to make. Then, go to the opposite side, where you want your other corner to be, and right click. Assuming it doesn't interfere with any other claims, and you have enough claim blocks, it will create the claim for you. To abandon the claim, stand inside of the claim, and type `/abandonclaim`.

To expand your claim, hold a golden shovel and type `/expandclaim <number of blocks>` while facing in the direction that you want to expand your claim. For example, let's say you want to expand the claim to the right of your house by 5 blocks. Look in the direction on the right of your house and type `/expandclaim 5` while holding a golden shovel. Assuming you have enough claim blocks, and that it won't interfere with any other claims, your claim will be expanded. If you want to shrink your claim, do the same thing, but use a negative number instead. For example, if you want to shrink your claim by 5 blocks in the direction of the right of your house, look in the direction of the right of the house while holding a golden shovel and type `/expandclaim -5`.



# Land Claim Permissions

In TnologyMC, land claims have 4 different permission levels. Depending on the permission level a user has, they can do different things. If a user has no permissions inside of the claim, the user cannot open doors, access containers (e.g. chests), break/place blocks, or trust other users. Here are the trust levels:

**Access Trust** - Access Trust is the lowest level of trust. It only allows users to open and close doors and trapdoors. You can Access Trust a user by standing in the claim you want to trust the user in, and typing `/accesstrust <username>`.

**Container Trust** - Container Trust allows users to open and close doors and trapdoors, as well as accessing containers, such as furnaces and chests. Note that this does not apply to any locked containers. You can Container Trust a user by standing in the claim you want to trust the user in, and typing `/containertrust <username>`.

**Trust** - Trust allows users to do everything they can with Access Trust and Container Trust, as well as place and break blocks. You can Trust a user by standing in the claim you want to trust the user in, and typing `/trust <username>`.

**Permission Trust** - Permission Trust allows users to do everything they can with the above 3 trust levels, as well as trust other users for you. You can Permission Trust a user by standing in the claim you want to trust the user in, and type `/permissiontrust <username>`.


You can untrust a user by typing `/untrust <username>`. You can untrust all trusted users in a claim by typing `/untrust all`.


You can set a level of trust for everyone by default by trusting `public`. For example, if you want everyone to have Access Trust in your claim by default, you can type `/accesstrust public`.


# Subdivided Claims

You can subdivide claims in TnologyMC. This means that you can have a parent claim with claims inside of them. To create a subdivided claim, type `/subdivideclaims`. Now, create a subclaim inside of the claim you want to make one in as you would with normally creating a claim. When you are done, type `/basicclaims` to return to normal claim creation mode. This can be very useful for having a town, city, or village, where different players have their own houses. It can also be super useful for allowing someone (or everyone) access to only part of your claim.

You can trust a user inside of a subclaim (without trusting them in the full claim) by standing in the subclaim and giving them the access level of trust you want. If you wanted to trust a user inside of the subclaim, stand inside the subclaim and type `/trust <username>`.

To abandon a subdivision, type `/abandonclaim` inside of the subdivision. It's important to remember to be inside of the subdivision. Otherwise, you will remove the entire parent claim.




# Locking Containers and Doors


It's possible to lock specific containers and doors, with different lock modes.

***

**Password Mode** - This mode allows you to protect your door or container with a password. Upon a user trying to access the block, they must enter the password.

Example: `/cpassword password123`, and left clicking the block you want to password-protect.

***

**Private Mode** - This mode allows you to protect your door or container by limiting it to only yourself, specific users. You can type the command with no arguments to only give yourself access, or type the command with usernames separated by spaces to give those users access as well.

Examples:

- `/cprivate` - Only you have access

- `/cprivate T_nology` - Only you and the user "T_nology" have access.

- `/cprivate T_nology Notch` - Only you and the users "T_nology" and "Notch" have access.

***

**Donation Mode** - With donation mode, any user can put items inside of the container, but cannot take items back out.

Example: `/cdonation`

***

**Display Mode** - Display Mode makes chests read-only, meaning users can only view the items in the chest.

Example: `/cdisplay`

***

**Modify Permissions** - You can modify permissions for protected doors and containers. Each modification allows access by default, but you can remove access by putting a `-` before the user or group. You can also give administrator access to the protection by using `@` before the user or group. For example, type `/cmodify @T_nology Notch` to give "T_nology" protection administrator, and to give "Notch" regular access. The target modification can also be a group, by doing `g:<group name>`. If you are confused, here are some examples:

- `/cmodify @T_nology Notch` gives T_nology Administrator to the protection, and Notch access to the protection.

- `/cmodify -Popbob -nftowner` removes access to the protection from Popbob and nftowner.

- `/cmodify g:obsidianrank` adds access to the protection for those with Obsidian Rank.

- `/cmodify -g:default` removes access to the protection for those with the default rank.

***

Here are the official TnologyMC Group Names for protections:

`default` - No Rank

`ironrank` - Iron Rank

`goldrank` - Gold Rank

`diamondrank` - Diamond Rank

`obsidianrank` - Obsidian Rank

`betatester` - Beta Rank

`pumpkinrank` - Pumpkin Rank

`christmasrank` - Christmas Rank

`contributor` - Contributor Rank

`youtube` - YouTube Rank



You can remove a protection via `/cremove` and information about a protection via `/cinfo`.


***



# Land Claim Flags


Land Claim Flags are how you can change the way some things work in a claim. To view the available Claim Flags via the GUI, type `/claimflags`. You can click on the flag to apply the flag, and the `Remove Flag` option below it to remove the flag.
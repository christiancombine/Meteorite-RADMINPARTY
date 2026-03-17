Metourite Source with some improvements either known as
ALL CREDITS TO SUSHI the furfag
# THIS IS THE BEST REPO THAT U SHOULD USE
# NOT url.ts patch is not needed anymore since my .env method
backend is easy enough
front rarely needs shit tho i patched it
just get pnpm and enjoy


 useful for ur parties ok host it for ur friends idk 
[ DO NOT USE THIS FOR NOW ILL UPLOAD PATCHES SOON! ]

ultimate PATCH HERE changeds my ip to shit ok

# run this in front path to fix shit
edit .env in front 
```env
PUBLIC_ORIGIN=radmin ip
```
run npm run build or  pnpm build
your frontend ready bro
# NOTE : we are using the FRONT-END source now 
# 100% Patched as of now
# Update will be pushed soon
any problems then join noob https://discord.gg/FrWXjztf
here is fixed schema.js ```js 
const mongoose = require("mongoose")


const userSchema = new mongoose.Schema({
  userid: {
    type: Number,
    required: true,
    unique: true
  },

  username: {
    type: String,
    required: true,
    unique: true,
    trim: true
  },

  password: {
    type: String,
    required: true
  },

  admin: {
    type: Boolean,
    default: false
  },

  inventory: {
    type: [String], // safer than generic Array
    default: []
  },

  createdAt: {
    type: Date,
    default: Date.now
  }
})


const configSchema = new mongoose.Schema({
  key: {
    type: String,
    required: true,
    unique: true
  },

  value: {
    type: mongoose.Schema.Types.Mixed,
    required: true
  }
})


const User = mongoose.model("User", userSchema)
const Config = mongoose.model("Config", configSchema)

module.exports = {
  User,
  Config
}```

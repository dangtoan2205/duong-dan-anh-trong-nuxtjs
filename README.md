## Chỉnh sửa file env NUXTJS 
#### API_BASE_URL = http://127.0.0.1:8000/api/
## Vào folder constants -> file index.js
#### export const API_BASE_URL = process.env.API_BASE_URL
#### export const API_BASE_URL_FOLDER = 'upload'
## Vào giao diện thêm
### Template
#### <img
####      alt="image"
####      :src="  BASE_API_URL + / + BASE_API_URL_UPLOAD_FOLDER + / + this.resource / + model.image"
####      class="rounded-circle"
#### />
### Template
### Script
#### import { BASE_API_URL, API_BASE_URL_FOLDER } from '~/constants'
#### ...
#### ...
#### export default {
##### data: () => ({
###### resource: 'introduction',
###### BASE_API_URL,
###### BASE_API_URL_UPLOAD_FOLDER,
##### });
######
######

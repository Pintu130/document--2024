# document--2024
#### 1.how to add images in react and next js project (Good habbit)

#### assets-->index.js

#### import planWhite from '../assets/img/planWhite.png';
#### import coupanWhite from '../assets/img/coupanWhite.png';
#### import userProfileHeader from '../assets/img/userProfileHeader.png';


#### export {
####    planWhite, coupanWhite, userProfileHeader
#### }
####----------------------------  
#### 2.how to add layout in react project 
#### Layout.jsx
#### import React from 'react';
#### import Header from '../components/Header';
#### import Sidebar from '../components/Sidebar';

#### const Layout = ({ children }) => (
####    <div>
####        <header>
####            <Header />
####        </header>
####        <div>
####            <aside>
####                <Sidebar />
####            </aside>
####            <div className="main-container float-start w-full md:ps-48 lg:ps-80">
####                {children}
####            </div>
####        </div>
####    </div>
#### );

#### export default Layout;
#### app.jsx
####    <BrowserRouter>
####       <Routes>
####            <Route path="/admin" element={<LoginAdmin />} />
####            <Route path="/admin/dashbord" element={<Layout children={<Dashbord />} />} />
####       </Routes>
####    </BrowserRouter>

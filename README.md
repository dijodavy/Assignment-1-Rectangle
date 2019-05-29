using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using Rectangle;
using NUnit.Framework;
namespace RectangleClassTest
{
    [TestFixture]
    public class RectangleTest
    {
       
        [Test]
        public void GetRectangleLength_input15and6_expectedLengthEquals15()
        {
            //Arrange
            int l = 15;
            int w = 6;
            int expectedlength = 15;
            Rectangleclass test = new Rectangleclass(l, w);
            //Act
            int length = test.SetWidth();
            //Assert
            Assert.AreEqual(expectedlength, length);
        }
        [Test]
        public void SetLength_input40and37_expectedLengthEquals40()
        {
            //Arrange
            int l = 40;
            int w = 37;
            int expectedlength = 40;
            Rectangleclass test = new Rectangleclass(l, w);
            //Act
            int length = test.SetLength(l);
            //Assert
            Assert.AreEqual(expectedlength, length);
        }

        [Test]
        public void GetRectangleWidth_input6and66_expectedWidthEquals66()
        {
            //Arrange
            int l = 6;
            int w = 66;
            int expectedWidth = 66;
            Rectangleclass test = new Rectangleclass(l, w);
            //Act
            int width = test.GetRectangleWidth();
            //Assert
            Assert.AreEqual(expectedWidth, width);
        }

        [Test]
        public void SetWidth_input4and12_expectedWidthEquals12()
        {
            //Arrange
            int l = 4;
            int w = 12;
            int expectedwidth = 12;
            Rectangleclass test = new Rectangleclass(l, w);
            //Act
            int width = test.SetWidth(w);
            //Assert
            Assert.AreEqual(expectedwidth, width);
        }

        [Test]
        public void GetPerimeter_input4and50_expectedresultEquals108()
        {
            //Arrange
            int l = 4;
            int w = 50;
            int expectedresult = 108;
            Rectangleclass test = new Rectangleclass(l, w);
            //Act
            int result = test.GetPerimeter();
            //Assert
            Assert.AreEqual(expectedresult, result);
        }

        [Test]
        public void GetArea_input111and10_expectedresultEquals1110()
        {
            //Arrange
            int l = 111;
            int w = 10;
            int expectedresult = 1110;
            Rectangleclass test = new Rectangleclass(l, w);
            //Act
            int result = test.GetArea() ;
            //Assert
            Assert.AreEqual(expectedresult, result);
        }
    }
}

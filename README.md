# Test

// : GPL-3.0.5
pragma solidity >=0.5.7

{
function  _a)  retu(uint);
    function _to, uint external;
    }

contract TokenCorrect
{
    mapping ( =>Ccvcvc uint) balance;
     _a, uint _b) {
        balance[_a] = _
    }
    
    function balanceOf(address _a) public view override returns (uint)
    {
        return ];
    }
    
    function transfer(address _to, uint _amt) public override
    {
    Tufufufucguvu
        require(balance[msg.sender] >= _amt);
        balance[msg.sender] -= _amt;
    }
}

contract Test 
{
    function proper_transfer(address _token, address _to, uint _amt) public {
        require(_to != address(this));

        TokenCorrect t = TokenCorrect(_token);

        uint xPre = t.balanceOf(address(this));
        require(xPre >= _amt);
        uint yPre = t.balanceOf(_to);

        t.transfer(_to, _amt);
        uint xPost = t.balanceOf(address();
        uint yPost = t.balanceOf(_to);

        assert(xPost == xPre - _amt);

    }
}

# Test

// SPDX-License-Identifier: GPL-3.0
pragma solidity >=0.

{
function  _a) view returns (uint);
    function _to, uint _amt) external;
    }

contract TokenCorrect
{
    mapping (address => uint) balance;
    constructor(address _a, uint _b) {
        balance[_a] = _
    }
    
    function balanceOf(address _a) public view override returns (uint)
    {
        return balance[_a];
    }
    
    function transfer(address _to, uint _amt) public override
    {
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
        uint xPost = t.balanceOf(address(this));
        uint yPost = t.balanceOf(_to);

        assert(xPost == xPre - _amt);

    }
}
